# FOUR WORLDS, ONE SQUAD — Technical Architecture

_Last updated: 2026-11-17_

## Objectives

Build a modular, mostly automated production pipeline for short-form episodes:
- Vertical 9:16 output for TikTok, Instagram Reels and YouTube Shorts.
- Target duration: 90 seconds; hard ceiling: 120 seconds.
- Human decisions remain required for creative approval and final quality control.
- Reuse the existing self-hosted La Nouvelle Carte n8n instance. Do not deploy a second n8n instance.
- Keep all FWS automation isolated in the n8n personal-project folder `FOUR WORLDS, ONE SQUAD`.

## n8n workflows

All seven workflows are created in the folder above. They are currently inactive.

| Workflow | Responsibility | Current state |
|---|---|---|
| `FWS - 01 - Episode Orchestrator` | Receives episode requests, validates the title, creates the episode record and launches script generation asynchronously. | Implemented; webhook is not activated. |
| `FWS - 02 - Script Generation` | Generates a structured French script with Groq GPT-OSS 120B, stores it and launches scene breakdown. | Implemented and tested. |
| `FWS - 03 - Scene Breakdown` | Converts the script into scenes, shot plans, visual prompts, camera directions and sound design; persists scenes and queues video jobs. | Implemented and tested. |
| `FWS - 04 - Asset Management` | Registers and versions character, location, prop and voice references. | Registry implemented. |
| `FWS - 05 - Video Generation` | Records one video-generation job per scene. | Queue implemented; provider adapter blocked. |
| `FWS - 06 - Post Production` | Records render requests for the FFmpeg worker. | Queue implemented; worker endpoint blocked. |
| `FWS - 07 - Quality Control & Delivery` | Checks video URI, duration, dimensions, vertical ratio and audio presence; blocks publication pending human review. | Implemented; failure path tested. |

### Workflow contracts

- The orchestrator accepts a JSON body with `title` (required), `synopsis` (optional), `format` (default `vertical_9_16`) and `targetDurationSeconds` (default `90`).
- A missing title is rejected with HTTP 400 before any episode record is written.
- A valid request is persisted and the script workflow is launched asynchronously. The orchestrator responds with HTTP 202.
- Script generation writes `scriptJson` and updates `scriptStatus`.
- Scene breakdown writes one row per scene and updates `sceneStatus`.
- Each scene creates a production job with `stage=video_generation`.
- QC only sets `ready_for_human_review` when a video URI exists, duration is between 1 and 120 seconds, dimensions are portrait with a 9:16 ratio (±0.02), and audio is explicitly confirmed. Otherwise it sets `technical_failed`.
- Publication remains `blocked_pending_human_review` until a human approval mechanism is added.

## n8n data tables

### `FWS - Episodes`
Episode-level metadata, request payload, generated script, stage statuses, QC result, final video URI, human review and publication status.

Important fields: `episodeId`, `title`, `status`, `format`, `targetDurationSeconds`, `synopsis`, `scriptJson`, `scriptMarkdown`, `scriptStatus`, `sceneStatus`, `qcStatus`, `qcNotes`, `finalVideoUri`, `humanReviewStatus`, `publicationStatus`.

### `FWS - Scenes`
One row per scene, including location, duration, dialogue, characters, visual prompt, camera direction, sound design, shot plan and generated video URI.

### `FWS - Assets`
Versioned registry for character, location, prop and voice references. Initial text profiles for Dylan and Li Wei are registered. Their image files are not stored in this table yet; `referenceUri` is intentionally blank until a real asset is uploaded.

### `FWS - Production Jobs`
Queue and status log for video generation and post-production jobs, including provider, scene ID, prompts, input/output URIs and error messages.

## AI providers

- Script and scene generation currently use the existing Groq API credential with model `openai/gpt-oss-120b`.
- The existing Gemini credential returned `401 API_KEY_SERVICE_BLOCKED` on the Gemini API. It is not used by the text-generation workflows.
- All generation prompts explicitly enforce the series' children-only universe: every human in the world is aged 0–12; no adults or teenagers may appear.
- Generated scripts and production descriptions must be in French.

## External production dependencies still to resolve

### Video generation: Google Flow

Google Flow is the preferred creative environment, but Google currently presents it as a web product and no official public Flow API integration is configured in this n8n instance.

References:
- Official product: https://labs.google/fx/tools/flow
- Third-party REST wrapper (not a Google product): https://github.com/useapi/google-flow-api

The video-generation workflow therefore records jobs as `blocked_external_adapter`. Do not activate an external paid wrapper or replace Flow with a different provider without an explicit decision.

### Post-production: FFmpeg

The post-production workflow records jobs as `blocked_worker_endpoint`. The local FFmpeg worker URL, authentication, media paths and shared storage contract still need to be configured. Do not assume that FFmpeg is installed inside the n8n container.

### Media storage

MinIO/S3 integration and stable URI conventions for character references, generated clips, voice tracks, subtitles and final exports are not yet connected.

## Security and activation

- All seven workflows remain inactive.
- The orchestrator webhook currently uses no authentication. Do not activate or expose it publicly until a dedicated inbound authentication method is configured.
- Do not reuse the Espo CRM credential for the FWS webhook.
- Do not publish any episode automatically. Final creative approval and final QC remain human-controlled.

## Validation performed

- Script generation through Groq succeeded and persisted structured JSON.
- Scene breakdown succeeded and created scene records with prompts and shot plans.
- Scene records successfully created one blocked video-generation job each.
- QC failure path correctly marked an episode as `technical_failed` and blocked publication.
- Temporary technical-test records were removed after validation.
