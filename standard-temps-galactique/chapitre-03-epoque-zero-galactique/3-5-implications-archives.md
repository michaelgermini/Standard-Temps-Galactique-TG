# 3.5 — Implications pour les archives et sites de stockage

L’adoption de l’EZG oblige à recalibrer les archives longue durée (déchets nucléaires, bibliothèques de sauvegarde, registres juridiques). Les actions recommandées sont :

1. **Double datation** : chaque artefact indique la date locale (ISO 8601, calendrier lunaire, etc.) ET la date TG (`EZG + HÉL + COS`). Cette redondance aide les futurs lecteurs à recouper les références.
2. **Mises à jour périodiques** : lors des inspections quinquennales, on vérifie que la version TG référencée reste cohérente (ex. : TG.v2025 → TG.v2030).
3. **Ancrage spatial** : les dépôts incluent une carte galactique simplifiée (Annexe A3) pour replacer l’EZG en contexte et éviter que l’information perde son sens si la Terre n’est plus connue.

## Cas particuliers

- **Déchets nucléaires** : les panneaux d’avertissement indiquent la durée minimale d’isolement en HÉL, ce qui offre un repère plus pertinent que “10 000 ans”, souvent incompréhensible pour une culture future.
- **Archives numériques** : les métadonnées EXIF, JSON ou XML reçoivent des champs `tg_hel`, `tg_cos`, etc., afin que les archives distribuées puissent se synchroniser automatiquement.

Grâce à ces mesures, le TG devient une couche supplémentaire de résilience documentaire plutôt qu’un remplacement brutal des systèmes existants.

