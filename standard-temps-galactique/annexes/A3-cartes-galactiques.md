# Annexe A3 — Cartes galactiques de référence

Cette annexe fournit les paramètres nécessaires pour reconstituer la géométrie de la Voie lactée.

## Projection plane (vue de dessus)

- Centre galactique à l’origine.
- Soleil placé à `(x, y) = (0, R₀)` avec `R₀ = 8,178 kpc`.
- Bras principaux modélisés par des spirales logarithmiques :

```
r = r₀ * e^{(θ - θ₀) * tan(p)}
```

où `p` est l’angle de pas (12° pour le bras de Persée, 13,5° pour Sagittaire).

## Profil (vue de tranche)

- Épaisseur du disque mince : ±300 pc.
- Épaisseur du disque épais : ±1 000 pc.
- Bulbe central : sphéroïde de demi-axe 1,5 kpc.

## Objets repères

| Objet | Coordonnées galactiques (l, b) | Remarque |
|-------|--------------------------------|----------|
| Pulsar B1937+21 | (57,5°, −0,3°) | Période 1,5578 ms (utilisé comme horloge naturelle). |
| Amas globulaire M13 | (59,0°, +40,9°) | Sert de balise visuelle. |
| Nuage moléculaire W51 | (49,5°, −0,4°) | Référence pour les cartes radio. |

## Illustrations fournies

- `illustrations/projection-plane.svg` : vue plane annotée (centre galactique, bras, position solaire).
- `illustrations/profil-disque.svg` : coupe du disque montrant bulbe, disque mince, halo.

Ces fichiers peuvent être gravés directement sur les couches MULS ou intégrés dans des présentations numériques. Ils servent également de base pour générer d’autres formats (PNG, STL) selon les besoins.

