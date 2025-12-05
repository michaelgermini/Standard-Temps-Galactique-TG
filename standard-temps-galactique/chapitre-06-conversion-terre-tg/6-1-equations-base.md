# 6.1 — Équations de conversion de base

Les conversions reposent sur trois étapes :

1. **Date terrestre → secondes SI**  
   - Utiliser le calendrier proleptique grégorien.  
   - Convertir en jours juliens (JD) puis en secondes : `s = (JD - JD₀) × 86 400`.
2. **Secondes SI → fraction de GY**  
   - `f = s / (GY_in_seconds)` où `GY_in_seconds = 230 000 000 × 31 556 926`.
3. **Fraction → unités hiérarchiques**  
   - `HÉL = floor(f × 10⁶)`  
   - `COS = floor((f × 10⁹) mod 10³)`  
   - `G = floor((f × 10¹¹) mod 10²)` etc.

## Formule compacte

```
TG = EZG + f × GY
```

où `EZG` représente l’offset négatif (section 3.2). Les conversions inverses suivent la chaîne hiérarchique en multipliant par les facteurs correspondants (1 G = 10⁻¹¹ GY, etc.).

Toutes ces équations sont fournies en pseudo-code dans l’annexe A4 pour faciliter l’implémentation dans divers langages (Python, Rust, C++).

