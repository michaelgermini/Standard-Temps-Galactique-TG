# Chapitre 4 — Protocoles SUCL et MULS pour la communication longue durée

L’unité de temps ne suffit pas : il faut aussi des protocoles pour encoder l’information de manière compréhensible après des dizaines de millénaires. Ce chapitre introduit **SUCL (Standard Universal Chrono-Lattice)** et **MULS (Macro Universal Layering System)**, deux cadres complémentaires qui assurent la lisibilité et l’interprétabilité des messages temporels.

## Contenu des sections associées

- **4.1 SUCL : concept et syntaxe** — structure de trames, hiérarchie temporelle, champs obligatoires.
- **4.2 Encodage fractal** — comment SUCL exploite un motif géométrique/radial pour être décodé sans clé.
- **4.3 MULS : taxonomie des couches** — classification des contenus (données scientifiques, narrations, avertissements).
- **4.4 Interopérabilité SUCL–MULS** — règles pour associer des temps TG à des couches physiques ou logicielles.
- **4.5 Résilience face à la dérive linguistique** — stratégie de redondance, iconographie, matériaux.

Le couple SUCL/MULS permet de transmettre le TG dans les Géodes mais aussi dans des protocoles numériques (balises, dépôts Git, API publiques).

## Exemple mathématique concret

Calcul de la taille minimale d’un motif SUCL :

```
Longueur = rayon_spirale × angle
```

Pour une gravure à rayon 5 cm couvrant 2 tours (angle = 4π), la spirale doit mesurer `≈ 62,8 cm`. Cette dimension garantit une lisibilité tactile même après érosion.

## Tableau de classification des protocoles

| Élément | Champ principal | Format recommandé | Support |
|---------|-----------------|-------------------|---------|
| SUCL Bloc Identité | `ID{}` | ASCII gravé / JSON | L1 |
| SUCL Bloc Temps | `TIME{}` | Décimal hiérarchique | L1/L2 |
| MULS L2 | Lexiques | Pictogrammes + translittération | L2 |
| MULS L3 | Données scientifiques | Markdown, LaTeX, CSV | L3 |
| MULS L4 | Narrations | Audio, texte multilingue | L4 |

## Encadrés spéciaux

- ⚠️ **Attention** : ne stockez jamais d’information critique uniquement dans une couche numérique (L5). Prévoir une redondance analogique.
- 💡 **Conseil** : utilisez des pictogrammes universels (spirales, atomes, pulsars) pour coder l’intention avant même toute lecture textuelle.
- ✓ **Bonnes pratiques** : incluez un test de cohérence (checksum ou puzzle géométrique) pour que les destinataires valident qu’ils lisent correctement SUCL.

## Synthèse & évaluation

- **À retenir** : SUCL décrit le temps, MULS organise la matière. Leur coordination évite les ambiguïtés.
- **Question rapide** : que se passe-t-il si une couche MULS est détruite ? Comment SUCL permet-il de déduire ce qui manque ?

