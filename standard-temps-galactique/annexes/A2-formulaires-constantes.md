# Annexe A2 — Formulaires et constantes physiques

## Constantes de base (TG.v2025)

| Symbole | Valeur | Unité |
|---------|--------|-------|
| R₀ | 8,178 kpc | distance Soleil–centre |
| Θ₀ | 229 km·s⁻¹ | vitesse tangentielle |
| GY | 230 000 000 ans | année galactique |
| µG | 7,26 s | microgalace |
| λ_HI | 21,106 cm | longueur d’onde de l’hydrogène neutre |

## Profils de halo recommandés

### Einasto

```
ρ(r) = ρ₀ * exp{ - (2/α) [ (r/r₀)^α - 1 ] }
α = 0,16 ; r₀ = 20 kpc
```

### Navarro-Frenk-White

```
ρ(r) = ρ₀ / [ (r/rₛ)(1 + r/rₛ)² ]
rₛ = 16 kpc
```

## Formules de conversion rapides

```
1 HÉL = 230 ans = 72 868 jours
1 COS = 84,0 jours = 7 257 600 s
1 G   = 0,84 jour = 72 576 s
1 µG  = 7,26 s
```

Ces constantes doivent accompagner chaque implémentation pour assurer la cohérence mondiale du TG.

