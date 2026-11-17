# Règles narratives et de production

## Format des épisodes
- Durée cible : environ 90 secondes ; maximum 2 minutes lorsque l'histoire le justifie.
- Format vertical 9:16, destiné à TikTok, Instagram Reels et YouTube Shorts.
- Univers visuel : animation 3D cinématographique cohérente avec les références validées.
- Tous les personnages ont entre 0 et 12 ans. Aucun adulte ne doit apparaître.

## Structure et écriture
- Accroche rapide, mise en place claire, développement, twist éventuel et fin mémorable.
- Chaque épisode raconte quelque chose de clair sans remplissage.
- Les quatre héros restent centraux, mais leur présence et leur importance varient selon les besoins de l'histoire.
- Les personnages secondaires apparaissent uniquement s'ils servent l'intrigue.
- Les intrigues longues sont planifiées ; les éléments non validés ne deviennent pas du canon.

## Storyboard et génération avec Flow MCP

### Une frame est une image-clé
- Chaque frame du storyboard est une image fixe de référence, pas un clip.
- Les images-clés servent d'image de début et d'image de fin d'une séquence animée.
- Chaque séquence doit donc avoir au minimum deux images-clés : état visuel initial et état visuel final.
- Les deux images doivent permettre une transition animée crédible : éviter les changements impossibles de position, de décor ou d'action.
- Les dialogues et mouvements intermédiaires sont décrits dans la fiche de séquence, pas supposés par l'image fixe.

### Ordre obligatoire des champs pour chaque frame
Chaque frame commence par ces quatre champs, dans cet ordre exact :

1. **What this frame shows:** description précise de l'image fixe : lieu, cadrage, nombre exact de personnages visibles, identité de chacun, positions, postures, expressions, objets et état de l'action.
2. **Film technique:** nom exact et identifiant d'une technique disponible dans le fichier officiel Flow MCP. Ne jamais inventer de technique.
3. **References:** maximum **3 références au total** par frame. Personnages, objets, lieux et autres images comptent tous dans cette limite. Ne sélectionner que les références nécessaires.
4. **Match previous frame (same character drawing, palette and style):** valeur booléenne explicite true ou false.

Ces quatre champs doivent apparaître avant tout prompt complémentaire ou note technique.

### Références des lieux et objets
- Le registre central des assets visuels est `bible/locations-and-props.md`.
- Tout lieu ou objet enregistré, visible et important dans une frame ou un shot doit être mentionné dans son champ **References** sous son nom exact.
- La limite de trois références reste absolue. Prioriser les assets visuellement déterminants ; décrire les autres personnages ou éléments depuis leur fiche canonique.
- Les références d'un asset ne sont utilisables comme références Flow qu'après sa création et sa validation dans Flow. Le registre décrit les assets à générer et ne prétend pas qu'ils existent déjà.

### Techniques de film
- Source officielle : https://github.com/GTAI-1/flow-mcp/blob/b64538ae8ab8d8dc1be07b7a8990554957d365bb/src/techniques.ts
- Choisir une technique compatible avec la séquence et les images de début/fin.
- Répéter la même technique sur les deux frames d'une même séquence afin de garder une intention de caméra cohérente.
- Les techniques de transition qui nécessitent first_frame et last_frame ne sont utilisées que pour une vraie transition.
- Une technique de caméra décrit le mouvement caméra entre les images ; elle ne doit pas contredire leur composition.

### Références et contrôle des personnages
- Maximum 3 références par frame, sans exception.
- Si plus de trois personnages sont visibles, référencer au maximum trois d'entre eux et décrire précisément les autres depuis la bible.
- Ne jamais prétendre qu'une référence existe dans Flow si elle n'a pas été créée ou vérifiée.
- Décrire explicitement le nombre exact de personnages visibles et nommer chacun.
- Chaque personnage apparaît une seule fois, sauf demande narrative explicite.
- Aucun clone, figurant, passant, adulte, silhouette humaine ou reflet humain non demandé.
- Les écrans, photos, miroirs et arrière-plans ne doivent pas introduire de personnages supplémentaires.
- Respecter les vêtements, coiffures, proportions, palettes et accessoires canoniques.

### Règle Match previous frame
- true : continuité visuelle voulue avec l'image précédente ; conserver dessin, palette, style, lumière et éléments de décor compatibles.
- false : nouvelle scène, nouveau lieu, ellipse temporelle ou changement volontaire de base visuelle.
- La première frame d'un épisode utilise false.
- Ne pas mettre true uniquement parce que le même personnage revient après une autre scène.

### Prompts et validation
- Le prompt de génération doit être cohérent avec les quatre champs.
- Décrire concrètement le nombre et l'identité des personnages, leur position et l'action figée.
- Ne pas demander à Flow d'inventer personnages, accessoires, textes ou actions non prévus.
- Limiter les textes lisibles aux éléments explicitement prévus ; si la typographie exacte est critique, prévoir un ajout en postproduction.
- Valider les images-clés avant de générer l'animation entre elles.

## Idées non validées
Une idée non confirmée reste une proposition et ne devient pas un élément canon de la série.
