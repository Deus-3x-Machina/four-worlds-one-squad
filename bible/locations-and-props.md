# Référentiel des lieux et objets visuels

Ce document est le registre central des décors et objets récurrents de **FOUR WORLDS, ONE SQUAD**. Il sert à créer des références visuelles maîtresses dans Flow et à conserver les mêmes formes, matériaux, couleurs, proportions et détails d'un plan à l'autre.

Le registre évolue avec la série. Un élément n'est considéré comme canonique qu'après validation de sa référence visuelle. Les descriptions de ce fichier sont les bases de génération ; elles ne signifient pas que les assets ont déjà été créés dans Flow.

## Règles d'utilisation

- Chaque asset possède un identifiant stable et un nom exact à réutiliser dans Flow.
- Générer les lieux et objets séparément des personnages, sauf si une image de référence combinée est explicitement nécessaire.
- Une fois validé, ne pas modifier le design d'un asset sans mettre à jour cette fiche et les épisodes concernés.
- Dans chaque **Frame** et chaque **Shot**, tout lieu ou objet enregistré qui est visuellement présent et important pour l'action doit figurer dans **References**, sous son nom exact.
- Les références restent limitées à **3 au total**. Choisir les trois assets les plus importants pour l'image ; décrire dans le prompt les autres éléments visibles à partir de cette fiche. Les personnages non référencés doivent être décrits depuis `bible/characters.md`.
- Les éléments de décor intégrés à un lieu (table, étagères, rangements, éclairage fixe) ne nécessitent pas chacun une référence séparée, sauf s'ils deviennent des objets narratifs distincts.
- Les accessoires génériques sans design distinctif (ex. téléphone ordinaire) sont décrits par convention dans le prompt et ne sont pas des assets autonomes.
- Ne jamais inventer un asset, un logo, une inscription ou un détail distinctif absent de cette fiche.
- Statuts possibles : **À générer**, **À valider**, **Validé Flow**, **À mettre à jour**.

## Conventions visuelles communes

- Format de référence : image propre, lisible, sans personnage, sans texte parasite et sans logo.
- Direction artistique : univers contemporain, animation 3D cinématographique, cohérent avec l'identité visuelle de la série.
- Les décors doivent être conçus pour le cadrage vertical 9:16, mais rester assez larges pour permettre des plans moyens et larges.
- Les lieux ne doivent contenir aucun adulte, enfant figurant, silhouette ou reflet humain.
- Les objets doivent être montrés seuls sur un fond simple ou dans une vue produit neutre, avec leurs détails clairement visibles.
- Les images maîtresses validées dans Flow deviennent les références prioritaires ; les descriptions textuelles servent à les compléter, pas à les contredire.

---

# 1. Lieux

## LOC-01 — QG du groupe

**Nom exact de référence Flow :** `LOC-01 — QG du groupe`  
**Statut :** À générer  
**Première apparition :** Saison 1, épisode 1 — séquences 1 et 5  
**Type :** repaire privé contemporain des quatre amis.

### Description visuelle canonique proposée

Un repaire privé compact, aménagé dans un espace contemporain à Paris. Il doit donner l'impression d'un lieu utilisé par quatre enfants débrouillards : fonctionnel, personnel, organisé sans être luxueux. Une grande table centrale sert de surface de réunion et de travail. Des étagères murales accueillent du matériel et des rangements. Quelques écrans intégrés ou posés sur un meuble peuvent être présents, mais leurs affichages restent abstraits et ne montrent jamais de personnes. Une porte sécurisée donne accès à la réserve attenante.

Palette sobre : gris doux, bois moyen, noir mat et touches discrètes de bleu froid. Éclairage intérieur maîtrisé, mélange de lumière pratique et d'une lumière ambiante douce. Matériaux crédibles, usure légère d'un lieu régulièrement utilisé, aucun logo ni décoration portant un texte lisible.

### Éléments fixes à conserver

- Table centrale, de forme rectangulaire, suffisamment grande pour réunir les quatre amis.
- Étagères murales et rangements intégrés.
- Un ou deux écrans sans contenu lisible ni visage.
- Porte sécurisée menant à la réserve.
- Même implantation générale, palette, matériaux et direction de lumière dans toutes les apparitions.

### Prompt maître de génération

```text
Créer un décor seul, sans aucun personnage : le QG privé des quatre jeunes héros de FOUR WORLDS, ONE SQUAD, situé à Paris. Espace contemporain compact, fonctionnel et crédible, conçu comme un repaire utilisé par quatre enfants inventifs. Grande table centrale rectangulaire, étagères murales, rangements, un ou deux écrans affichant uniquement des formes abstraites, porte sécurisée visible donnant sur une réserve attenante. Palette gris doux, bois moyen, noir mat et petites touches de bleu froid. Éclairage cinématographique doux, matériaux réalistes, légère patine d'usage, composition claire et exploitable en vidéo verticale 9:16. Aucun personnage, aucune silhouette, aucun reflet humain, aucun logo, aucun texte lisible, aucune marque.
```

### Invariants et interdits

- Le QG et la réserve sont deux espaces distincts, même s'ils sont directement attenants.
- Ne pas transformer le QG en laboratoire high-tech, manoir, bureau d'entreprise ou salle de contrôle futuriste.
- Ne pas ajouter de fenêtres panoramiques ou d'éléments architecturaux spectaculaires sans décision ultérieure.
- Ne jamais afficher de personnes sur les écrans.

---

## LOC-02 — Réserve de la Plata

**Nom exact de référence Flow :** `LOC-02 — Réserve de la Plata`  
**Statut :** À générer  
**Première apparition :** Saison 1, épisode 1 — séquences 6 à 9  
**Type :** pièce de stockage sécurisée attenante au QG.

### Description visuelle canonique proposée

Petite pièce de stockage fermée par une porte sécurisée, accessible directement depuis le QG. L'espace est pratique et organisé, pas une chambre forte bancaire. Il contient plusieurs étagères solides, des boîtes, des compartiments et des zones de rangement. Dans l'épisode 1, tous ces rangements sont vides : la Plata est un ensemble de trésors et de biens accumulés, pas un objet unique.

La serrure et le mécanisme de fermeture doivent être visibles et crédibles. La porte ne présente aucune trace d'effraction. Palette cohérente avec le QG : gris, métal sombre, bois sobre, lumière intérieure légèrement plus froide et moins abondante.

### Éléments fixes à conserver

- Porte sécurisée donnant sur le QG.
- Serrure mécanique visible, intacte dans l'épisode 1.
- Étagères et compartiments de stockage.
- Même géométrie de pièce et même implantation entre les frames et shots.
- Dans l'épisode 1, tous les emplacements sont vides ; ne pas montrer un coffre unique contenant toute la Plata.

### Prompt maître de génération

```text
Créer un décor seul, sans personnage : une petite réserve privée sécurisée attenante au QG de quatre enfants. Ce n'est pas une chambre forte bancaire. Pièce de stockage compacte et organisée avec plusieurs étagères solides, boîtes de rangement, compartiments et une porte sécurisée équipée d'une serrure mécanique clairement visible. Montrer les rangements entièrement vides. Palette gris neutre, métal sombre et bois sobre, lumière cinématographique légèrement froide, espace réaliste et lisible en format vertical 9:16. La porte et la serrure ne présentent aucune trace d'effraction. Aucun personnage, silhouette, reflet humain, logo, texte ou coffre central représentant un trésor unique.
```

### Invariants et interdits

- La réserve doit rester la même pièce à chaque plan.
- La serrure est intacte dans l'épisode 1.
- Les biens disparus ne sont pas remplacés par un coffre unique ou un artefact unique.
- Ne pas ajouter de fenêtres, d'alarme spectaculaire ou de technologie biométrique sans validation.

---

## LOC-03 — Salon de Mathis

**Nom exact de référence Flow :** `LOC-03 — Salon de Mathis`  
**Statut :** À générer  
**Première apparition :** Saison 1, épisode 1 — séquence 2  
**Type :** petit salon contemporain.

### Description visuelle canonique proposée

Un petit salon contemporain, simple et confortable, dans lequel Mathis peut être assis sur un canapé puis se lever rapidement. Décor quotidien, chaleureux et peu chargé. Canapé deux ou trois places, petite table basse et quelques éléments domestiques sobres. La pièce ne doit pas paraître luxueuse ni particulièrement technologique.

Palette douce et légèrement chaude : beige, crème, bois clair et quelques touches de vert compatibles avec la tenue de Mathis. Prévoir une sortie clairement identifiable dans le cadre pour son départ.

### Prompt maître de génération

```text
Créer un petit salon contemporain et chaleureux, vide de tout personnage, pour la série FOUR WORLDS, ONE SQUAD. Un canapé deux ou trois places clairement visible, une petite table basse, quelques éléments domestiques sobres, décoration discrète et crédible. Palette beige, crème, bois clair et petites touches de vert. Espace simple, confortable, non luxueux, avec une sortie clairement identifiable sur un côté du cadre. Lumière intérieure douce et naturelle, composition cinématographique adaptée au format vertical 9:16. Aucun personnage, silhouette, reflet humain, logo ou texte lisible.
```

### Invariants et interdits

- Conserver le même canapé, la même table basse et la même sortie entre les deux frames.
- Ne pas ajouter de colocataire, animal ou autre personnage.
- Ne pas transformer le salon en chambre ou en grand appartement luxueux.

---

## LOC-04 — Zone d'arrivée de l'aéroport de Paris

**Nom exact de référence Flow :** `LOC-04 — Aéroport de Paris, zone d'arrivée`  
**Statut :** À générer  
**Première apparition :** Saison 1, épisode 1 — séquence 3  
**Type :** terminal d'aéroport contemporain.

### Description visuelle canonique proposée

Zone d'arrivée d'un aéroport parisien contemporain, stylisée mais crédible, avec grandes baies vitrées, architecture claire et circulation piétonne lisible. Le décor doit pouvoir être utilisé sans montrer de voyageurs, employés ou personnel. L'image doit évoquer un aéroport sans dépendre de logos, de noms de compagnies ou de panneaux lisibles.

Palette neutre : verre, métal clair, pierre grise et lumière naturelle froide. Prévoir un espace dégagé permettant à Zayd de marcher avec une petite valise cabine et de faire demi-tour.

### Prompt maître de génération

```text
Créer un décor vide de zone d'arrivée d'un grand aéroport parisien contemporain, sans aucun être humain. Architecture moderne et crédible, grandes baies vitrées, structure métallique claire, sol en pierre grise, lumière naturelle légèrement froide, espace de circulation dégagé permettant à un enfant avec une petite valise cabine de marcher puis de faire demi-tour. Ambiance aéroportuaire reconnaissable mais sans logo, nom de compagnie, panneau lisible ni marque. Composition cinématographique verticale 9:16. Aucun voyageur, employé, adulte, enfant figurant, silhouette ou reflet humain.
```

### Invariants et interdits

- Même terminal, même lumière et même architecture dans les deux frames.
- Aucun voyageur, employé, personnel ou reflet humain.
- Aucun logo ou texte d'aéroport généré.

---

## LOC-05 — Atelier technologique de Li

**Nom exact de référence Flow :** `LOC-05 — Atelier technologique de Li`  
**Statut :** À générer  
**Première apparition :** Saison 1, épisode 1 — séquence 4  
**Type :** petit atelier personnel d'électronique et de robotique.

### Description visuelle canonique proposée

Atelier compact et ordonné, dédié à l'électronique et à la robotique. Un établi principal occupe le premier plan. Il comporte un tapis de travail, quelques outils de précision, des composants électroniques et des rangements organisés. Le petit robot mécanique de Li est posé sur l'établi (l'objet possède sa propre référence PROP-03).

L'atelier est technologique mais reste réaliste et à l'échelle d'un enfant passionné. Palette gris clair, noir, métal brossé et lumière froide maîtrisée. Aucun écran ne montre de visage ou de personnage.

### Prompt maître de génération

```text
Créer un petit atelier personnel d'électronique et de robotique, vide de tout personnage, pour un jeune inventeur. Établi principal au premier plan avec tapis de travail, outils de précision, composants électroniques soigneusement rangés et petits bacs de rangement. Quelques écrans techniques affichant uniquement des schémas abstraits, jamais de visage. Ambiance technologique crédible, organisée et à échelle humaine, pas un laboratoire futuriste. Palette gris clair, noir et métal brossé, éclairage froid doux et cinématographique, composition verticale 9:16. Aucun personnage, silhouette, reflet humain, logo ou texte lisible.
```

### Invariants et interdits

- Conserver l'établi et son implantation.
- Le robot est un objet séparé, référencé PROP-03.
- Ne pas ajouter d'assistant, de second robot humanoïde ou de personnage sur les écrans.

---

# 2. Objets et accessoires narratifs

## PROP-01 — Téléphone personnel générique

**Nom exact de référence Flow :** `PROP-01 — Téléphone personnel`  
**Statut :** À générer si un modèle maître commun est nécessaire ; sinon convention de prompt  
**Première apparition :** Saison 1, épisode 1 — séquences 1 à 4  
**Type :** smartphone contemporain sans marque.

### Description visuelle

Smartphone moderne de taille adaptée à la main d'un enfant, écran tactile noir brillant, bords fins, coque unie sombre sans logo. Le modèle reste générique afin de pouvoir être utilisé par les quatre personnages. L'écran peut afficher une interface abstraite de notification ou d'appel, mais aucun texte lisible ne doit être inventé.

### Prompt maître de génération

```text
Smartphone contemporain générique, sans marque ni logo, taille adaptée à la main d'un enfant, écran tactile noir brillant, bords fins, coque unie gris anthracite ou noire mate, design sobre et crédible. Vue produit isolée, face avant et dos visibles, écran sans texte lisible et sans notification contenant des mots. Aucun accessoire supplémentaire.
```

### Invariants et interdits

- Même silhouette générale et même finition lorsqu'il est utilisé comme accessoire de continuité.
- Aucun logo, marque ou texte inventé.
- Les interfaces et notifications peuvent être ajoutées en postproduction si leur contenu exact est important.

---

## PROP-02 — Valise cabine de Zayd

**Nom exact de référence Flow :** `PROP-02 — Valise cabine de Zayd`  
**Statut :** À générer  
**Première apparition :** Saison 1, épisode 1 — séquence 3  
**Type :** petite valise cabine premium et discrète.

### Description visuelle

Valise cabine compacte à coque rigide, finition sobre et premium, sans marque visible. Couleur gris clair métallisé ou champagne très discret, poignée télescopique sombre et quatre roulettes. Elle doit être assez petite pour être tirée par Zayd sans masquer son corps. Aucun autocollant ni étiquette lisible.

### Prompt maître de génération

```text
Valise cabine compacte à coque rigide, design premium discret, couleur gris clair métallisé avec finition légèrement satinée, poignée télescopique noire, quatre roulettes multidirectionnelles, poignée supérieure intégrée, aucune marque, aucun logo, aucun autocollant ni texte. Vue produit isolée en trois-quarts, proportions réalistes et adaptées à un enfant.
```

### Invariants et interdits

- Même couleur, forme, poignée et nombre de roulettes dans les deux frames.
- Pas de marque de luxe ni d'autocollant.

---

## PROP-03 — Petit robot mécanique de Li

**Nom exact de référence Flow :** `PROP-03 — Petit robot mécanique de Li`  
**Statut :** À générer  
**Première apparition :** Saison 1, épisode 1 — séquence 4  
**Type :** petit prototype robotique inanimé.

### Description visuelle proposée

Petit prototype mécanique posé sur l'établi de Li. Forme compacte, principalement composée de pièces métalliques et de coques gris clair/noir. Il doit évoquer un prototype électronique construit et entretenu par un enfant passionné, sans ressembler à un personnage. Pas de visage, pas d'yeux expressifs, pas de bouche, pas de bras humanoïdes. Quelques connecteurs, vis apparentes et capteurs simples peuvent être visibles.

### Prompt maître de génération

```text
Petit prototype robotique mécanique inanimé, objet seul posé sur un établi ou présenté en vue produit. Forme compacte et technique, assemblage de coques gris clair et noir, quelques pièces métalliques, vis apparentes, petits connecteurs et capteurs simples. Design crédible de prototype électronique construit par un jeune passionné. Il ne doit absolument pas ressembler à un personnage : aucun visage, aucun œil expressif, aucune bouche, aucune expression, aucune silhouette humanoïde, aucun bras ou jambes de robot. Aucun logo ni texte.
```

### Invariants et interdits

- Le robot reste un objet inanimé dans l'épisode 1.
- Conserver sa forme, ses couleurs, ses capteurs et ses proportions.
- Ne jamais le faire parler, marcher ou exprimer une émotion.
- Ne pas le transformer en robot humanoïde.

---

## PROP-04 — Serrure de la réserve

**Nom exact de référence Flow :** `PROP-04 — Serrure de la réserve`  
**Statut :** À générer  
**Première apparition :** Saison 1, épisode 1 — séquence 7  
**Type :** serrure mécanique de porte sécurisée.

### Description visuelle

Serrure mécanique compacte intégrée à la porte de la réserve, finition métal brossé sombre, cylindre et poignée sobres. Elle doit être assez détaillée pour permettre un plan rapproché d'inspection. Dans l'épisode 1, elle est intacte : pas de rayure forcée, pas de métal tordu, pas de trace d'outil, pas de pièce cassée.

### Prompt maître de génération

```text
Serrure mécanique compacte intégrée à une porte sécurisée intérieure, finition métal brossé sombre, cylindre de serrure et poignée sobres, détails mécaniques crédibles, vue rapprochée nette et lisible. La serrure est intacte, propre, sans rayure, sans trace d'effraction, sans métal tordu ni pièce cassée. Aucun logo, aucune marque, aucun texte.
```

### Invariants et interdits

- Même modèle et même finition dans tous les plans de la réserve.
- Dans l'épisode 1, la serrure n'a pas été forcée.
- Ne pas ajouter de clavier numérique, lecteur biométrique ou dispositif futuriste.

---

## PROP-05 — Carte manuscrite de Tony

**Nom exact de référence Flow :** `PROP-05 — Carte manuscrite de Tony`  
**Statut :** À générer ; texte à ajouter en postproduction si nécessaire  
**Première apparition :** Saison 1, épisode 1 — séquences 7 à 9  
**Type :** petite carte papier laissée dans la réserve.

### Description visuelle

Petite carte rectangulaire en papier épais, légèrement crème, sans illustration ni symbole. Aspect simple et volontairement anonyme. Une seule inscription manuscrite est prévue :

**« Toujours un coup d'avance. — T »**

La carte ne doit pas introduire un emblème, une signature graphique ou un symbole qui n'a pas été décidé dans la bible.

### Prompt maître de génération

```text
Petite carte rectangulaire en papier épais légèrement crème, surface mate, bords nets, aspect simple et anonyme. Vue de face, seule sur un fond neutre. Aucun dessin, aucun symbole, aucun logo, aucune bordure décorative. Prévoir une surface suffisamment propre pour ajouter en postproduction une seule inscription manuscrite : « Toujours un coup d'avance. — T ». Si le texte généré risque d'être incorrect, produire une carte totalement vierge.
```

### Invariants et interdits

- Même taille, couleur et texture papier dans tous les plans.
- Seul texte autorisé : « Toujours un coup d'avance. — T ».
- Aucun symbole de Tony n'est défini à ce stade.
- Préférer une carte vierge et ajouter le texte en postproduction si Flow déforme les caractères.

---

# 3. Références à utiliser dans l'épisode 1

Les noms exacts ci-dessous doivent être utilisés dans les champs **References** des frames et des shots concernés.

| Identifiant | Nom exact | Éléments concernés |
|---|---|---|
| LOC-01 | QG du groupe | QG, table centrale, étagères, écrans, porte de la réserve |
| LOC-02 | Réserve de la Plata | Réserve, étagères vides, compartiments, porte |
| LOC-03 | Salon de Mathis | Canapé, table basse, sortie |
| LOC-04 | Aéroport de Paris, zone d'arrivée | Terminal, baies vitrées, zone de circulation |
| LOC-05 | Atelier technologique de Li | Établi, outils, composants et rangements |
| PROP-01 | Téléphone personnel | Téléphone générique lorsqu'il est un élément important du plan |
| PROP-02 | Valise cabine de Zayd | Valise de Zayd |
| PROP-03 | Petit robot mécanique de Li | Prototype posé sur l'établi |
| PROP-04 | Serrure de la réserve | Gros plans et inspection de la serrure |
| PROP-05 | Carte manuscrite de Tony | Carte trouvée dans la réserve |

## 4. Journal des mises à jour

| Date | Modification | Statut |
|---|---|---|
| 2026-11-17 | Création du registre initial : 5 lieux et 5 objets pour l'épisode 1. | Références textuelles créées ; assets Flow à générer et valider |

## 5. Prochaines extensions

Ajouter ici les lieux et objets au fur et à mesure de leur apparition dans les épisodes. Avant de créer un nouvel asset, vérifier si un lieu ou objet existant peut être réutilisé. Ne créer une nouvelle référence que si ses caractéristiques visuelles ou son rôle narratif le justifient.
