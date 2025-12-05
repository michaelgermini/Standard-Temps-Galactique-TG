# 6.4 — Erreurs cumulatives et corrections

Les conversions Terre ↔ TG sont sensibles à plusieurs sources d’erreur :

1. **Variation de GY** : si la valeur de la période orbitale change (cf. chapitre 1.4), les conversions historiques doivent préciser la version. La différence se corrige en recalculant `GY_SECONDS`.
2. **Accumulation numérique** : sur de longues séries, les arrondis flottants peuvent introduire des biais. Utiliser des entiers (BigInt) ou des rationnels pour stocker les fractions.
3. **Desynchronisation d’horloges** : les horloges terrestres (TAI, UTC) subissent des secondes intercalaires. Les convertisseurs doivent intégrer les tables IERS.

## Stratégie de correction

- Publier des **patches TG** à chaque changement de version, contenant les facteurs de correction (`ΔGY`, `ΔEZG`).
- Conserver les données brutes (seconds SI) pour permettre des reconversions ultérieures.
- Documenter la précision effective d’un enregistrement via le champ SUCL `P_ERR`.

En adoptant ces pratiques, les dates TG restent traçables malgré l’évolution des modèles astrophysiques et des technologies de mesure.

