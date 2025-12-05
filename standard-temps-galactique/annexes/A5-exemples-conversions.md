# Annexe A5 — Exemples de conversions et cas de test

Cette annexe fournit des cas concrets pour valider les implémentations.

| # | Date ISO (UTC) | Description | Résultat TG |
|---|----------------|-------------|-------------|
| 1 | 2000-01-01 12:00 | Référence J2000 | `EZG + HÉL 008.700 | COS 000 | G 00` |
| 2 | 2025-11-21 00:00 | Adoption officielle | `EZG + HÉL 008.742 | COS 511 | G 92` |
| 3 | 2025-12-31 00:00 | HÉL + 1 | `EZG + HÉL 008.743 | COS 000 | G 00` |
| 4 | 2525-01-01 00:00 | Projection +500 ans | `EZG + HÉL 010.913 | COS 102 | G 11` |

## Script de vérification

```
for case in test_cases:
    tg = terre_to_tg(case.date)
    assert close_enough(tg, case.expected, tolerance=1 micro)
```

## Documents de référence

- Table CSV (`annexes/donnees/tg-cases.csv`) listant des événements réels et prospectifs. Elle peut servir de base à vos propres ajouts (ajoutez des lignes en conservant la structure).
- Fichiers SUCL prêts à graver pour servir d’étalons physiques.

En utilisant ces exemples, les équipes garantissent que leurs convertisseurs et leurs archives restent compatibles avec le standard.

