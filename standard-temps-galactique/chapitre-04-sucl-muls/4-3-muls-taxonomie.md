# 4.3 — MULS : Macro Universal Layering System

MULS complète SUCL en définissant comment les informations sont superposées. Il s’agit d’une **taxonomie de couches** à la fois physiques (dans une Géode) et logiques (dans un fichier numérique).

| Couche | Nom | Contenu | Exemple |
|--------|-----|---------|---------|
| L0 | Support brut | matériau, géométrie, orientation | plaque en carbure de tungstène |
| L1 | SUCL Core | timecode, version, coordonnées | spirale gravée + champs textuels |
| L2 | Lexiques | pictogrammes, glossaires multilingues | table de correspondance symboles ↔ concepts |
| L3 | Données scientifiques | équations, constantes, cartes | définitions du TG, cartes galactiques |
| L4 | Narrations | contextes culturels, témoignages | histoire du TG, raisons politiques |
| L5 | Interfaces | instructions pour accéder aux formats numériques | QR, schémas de circuits |

## Règles de construction

1. Les couches doivent être lisibles indépendamment : un destinataire qui accède seulement à L1 doit déjà comprendre le temps.
2. L’ordre L0 → L5 ne peut être inversé : la lecture progressive limite les malentendus.
3. Chaque couche référence la précédente via des pictogrammes ou checksums pour garantir la cohérence.

MULS permet donc de construire des artefacts qui restent intelligibles même si certaines couches sont abîmées ou perdues.

