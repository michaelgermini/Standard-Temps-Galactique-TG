# 1.2 — Orbite solaire : rayon, vitesse et période

La période orbitale moyenne du Soleil définit l’année galactique (GY). Elle résulte de trois paramètres principaux :

| Symbole | Valeur de référence | Incertitude (1σ) | Source |
|---------|--------------------|-------------------|--------|
| R₀ (distance Soleil–centre) | 8,178 kpc | ±0,013 kpc | Collaboration Gravity, 2019 |
| Θ₀ (vitesse tangentielle) | 229 km·s⁻¹ | ±6 km·s⁻¹ | Gaia EDR3 + masers VLBI |
| P (période) | 230 Myr | ±20 Myr | dérivé de 2πR₀ / Θ₀ |

Ces valeurs combinent des mesures VLBI (masers méthanol/eau), l’accélération solaire observée par GRAVITY et les vitesses propres Gaia. L’incertitude dominante provient des variations de Θ₀ liées aux ondes de densité.

## Méthodologie de calcul

1. **Estimation de R₀** : on triangule la position de Sagittarius A* via la précession des étoiles S2/S62. La distance en kpc se convertit ensuite en mètres selon le SI.
2. **Mesure de Θ₀** : on moyenne la vitesse tangentielle d’étoiles jeunes (tracées par masers) dont les orbites sont proches du plan galactique, pour limiter la dispersion due aux vitesses aléatoires.
3. **Propagation des incertitudes** : le standard TG adopte une incertitude relative de 8,7 % sur la période, stockée comme méta-donnée dans tous les calculateurs (Annexe A4).

La valeur `1 GY = 230 000 000 ans terrestres` reste une moyenne. Toute institution peut recalculer la période avec les équations fournies en annexe A4, mais doit publier la version (`TG.vYYYY`) utilisée pour éviter les ambiguïtés historiographiques.

