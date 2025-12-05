# Annexe A7 — Formules et calculs détaillés

Cette annexe illustre pas à pas les calculs mentionnés dans le traité afin de servir de référence pédagogique.

## A7.1 Calcul de la période galactique

1. Conversion de R₀
   ```
   R₀ = 8,178 kpc = 8,178 × 3,085677581×10¹⁹ m
      = 2,524×10²⁰ m
   ```
2. Conversion de Θ₀
   ```
   Θ₀ = 229 km·s⁻¹ = 2,29×10⁵ m·s⁻¹
   ```
3. Période
   ```
   P = 2πR₀ / Θ₀
     = 2π × 2,524×10²⁰ / 2,29×10⁵
     = 6,93×10¹⁵ s ≈ 220 à 240 Myr (selon les incertitudes)
   ```

## A7.2 Propagation des incertitudes

Pour des valeurs `R ± ΔR` et `Θ ± ΔΘ`, l’incertitude relative de P est :

```
ΔP/P = √[(ΔR/R)² + (ΔΘ/Θ)²]
```

Avec `ΔR = 0,013 kpc` et `ΔΘ = 6 km·s⁻¹`, on obtient `ΔP ≈ 8,7 %`.

## A7.3 Exemple complet Terre → TG

Date : 2025‑11‑21 00:00 UTC.

1. `JD = 2460637.5`
2. `JD_EZG = JD_2025 - 0,0001356 × GY_en_jours`
3. `s = (JD - JD_EZG) × 86 400 = 2,187×10¹⁵ s`
4. `fraction = s / GY_seconds = 8,742×10⁻⁶`
5. `HÉL = floor(8,742×10⁻⁶ × 10⁶) = 8`
6. `COS = floor(8,742×10⁻⁶ × 10⁹) mod 1000 = 742`
7. `G = floor(8,742×10⁻⁶ × 10¹¹) mod 100 = 37`

## A7.4 Conversion inverse TG → Terre

Pour `EZG + HÉL 008.900 | COS 125 | G 50` :

1. `fraction = (8 + 0,125 + 0,0050) × 10⁻⁶ = 8,130×10⁻⁶`
2. `seconds = fraction × GY_seconds = 1,997×10¹⁵ s`
3. `JD = seconds / 86 400 + JD_EZG`
4. Conversion finale vers ISO (voir chapitre 6.2).

## A7.5 Modèle énergétique d’une Géode

Pour prédire la longévité des supports, on utilise la loi d’Arrhenius :

```
MTTF = A × exp(Ea / (k × T))
```

avec `A = 1,5×10⁶`, `Ea = 0,8 eV`, `T = 250 K`. On obtient `MTTF ≈ 4,2×10⁵ ans`, ce qui respecte l’objectif > 0,5 HÉL.

Cette annexe peut être complétée par vos propres calculs (ex : dynamique de bras, synchronisation de pulsars). N’oubliez pas de mentionner la version TG utilisée et les incertitudes associées.

