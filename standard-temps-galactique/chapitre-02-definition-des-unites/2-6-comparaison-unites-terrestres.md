# 2.6 — Comparaison avec les unités terrestres

Cette section aide les utilisateurs à naviguer entre le TG et les systèmes existants (SI, calendriers civils).

## Table de correspondance (TG.v2025)

| Unité TG | Durée terrestre approx. | Équivalent usuel |
|----------|------------------------|------------------|
| 1 GY | 230 000 000 ans | Orbite solaire galactique |
| 1 HÉL | 230 ans | Cycle civilisationnel |
| 1 COS | 84,0 jours | “Mois” galactique |
| 1 Galace | 20,1 h | Journée opérationnelle |
| 1 sG | 12,1 min | Session de briefing |
| 1 µG | 7,26 s | Étalon instrumental |

## Recommandations de conversion

1. **Toujours passer par le SI** (secondes) lors de conversions automatisées pour éviter les accumulations d’arrondis.
2. **Documenter les conventions calendaires** : lorsqu’on convertit une date ISO 8601, préciser si l’on utilise un calendrier proleptique grégorien ou julien.
3. **Publier des tables périodiques** : les annexes (A5) fournissent des exemples de conversions pour des événements historiques clés (J2000, lancement de la Géode, adoption du TG).

## Outils logiciels

- Bibliothèque `tg-convert` (pseudo-code en annexe A4) : convertit secondes SI → TG hiérarchique.
- Script `tg-cal` : produit des calendriers COS/G pour une année terrestre donnée.
- Spécification JSON pour inclure les métadonnées TG dans des API publiques.

Grâce à ces correspondances, les institutions peuvent déployer le référentiel galactique sans abandonner leurs systèmes locaux.

