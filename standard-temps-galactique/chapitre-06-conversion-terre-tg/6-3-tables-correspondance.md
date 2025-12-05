# 6.3 — Tables de correspondance historiques

Les tables facilitent la vérification humaine et les audits. Exemples (TG.v2025) :

| Événement | Date terrestre | Coordonnées TG |
|-----------|----------------|----------------|
| J2000 | 2000-01-01 12:00 UTC | `EZG + HÉL 008.700 | COS 000 | G 00` |
| Adoption officielle du TG | 2025-11-21 | `EZG + HÉL 008.742 | COS 512 | G 37.4` |
| Premier HÉL+1 | 2025-12-31 00:00 UTC | `EZG + HÉL 008.743 | COS 000 | G 00` |

## Construction des tables

1. Choisir des événements à haute valeur symbolique (scientifiques, culturels, juridiques).
2. Convertir via l’algorithme section 6.2.
3. Publier le résultat avec les incertitudes et la version `TG.vYYYY`.

## Formats recommandés

- **CSV** pour l’archivage simple.
- **JSON-LD** pour les API et les graphes de connaissances.
- **Gravure analogique** dans les Géodes (Annexe A5) pour assurer la lecture future.

Ces tables servent aussi d’unit tests pour les logiciels de conversion.

