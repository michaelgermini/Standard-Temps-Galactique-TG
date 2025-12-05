# 3.2 — Reconstruction géométrique de l’EZG

La reconstruction rétrograde de l’orbite solaire s’effectue en intégrant l’équation du mouvement dans le potentiel galactique (barre + disque + halo). Les étapes clés :

1. **Paramétrer le potentiel** : utiliser les constantes de la section 1 (R₀, Θ₀, profil de halo Einasto).
2. **Intégrer numériquement** : appliquer une méthode symplectique (Leapfrog, Runge-Kutta 4/5) sur 40 Myr afin d’identifier l’instant où la longitude galactique du Soleil est nulle.
3. **Appliquer les corrections relativistes** : pour les intégrations supérieures à 10⁸ ans, ajouter la précession induite par les masses concentrées du bulbe.

Le résultat majoritaire TG.v2025 situe l’EZG à **−31,2 Myr** par rapport à 2025. La date précise se note `EZG = −0,0001356 GY` dans la nomenclature TG.

## Validation croisée

- Comparaison avec les simulations cosmologiques (Illustris, EAGLE) pour s’assurer que le mouvement obtenu reste plausible.
- Vérification par les couches sédimentaires terrestres : certains isotopes cosmogéniques (¹⁰Be, ⁶⁰Fe) montrent des pics alignés avec le passage par des bras denses, fournissant des marqueurs indépendants.

Les scripts d’intégration de référence sont fournis en pseudo-code dans `annexes/A4-norme-iso-tg.md`.

