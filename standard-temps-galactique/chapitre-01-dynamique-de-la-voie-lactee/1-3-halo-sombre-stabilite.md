# 1.3 — Halo de matière noire et stabilité des trajectoires

La rotation quasi plate des galaxies spirales implique une distribution de masse étendue au-delà du disque lumineux : le **halo de matière noire**. Dans la Voie lactée, ce halo représente ~90 % de la masse gravitationnelle totale. Il suit une distribution proche d’un profil NFW (Navarro-Frenk-White) ou Einasto selon les modèles.

## Pourquoi le halo compte pour le TG

1. **Stabilité de la vitesse tangentielle** : l’excès de masse dans le halo maintient Θ₀ quasi constant jusqu’à ~20 kpc, garantissant que l’année galactique ne varie pas brutalement lorsque le Soleil traverse différents bras.
2. **Réduction des perturbations locales** : sans halo, chaque nuage moléculaire géant pourrait ralentir ou accélérer significativement l’orbite solaire. Le halo agit comme “tampon” dynamique.
3. **Mesurabilité à long terme** : les modèles de halo peuvent être recalibrés via courbes de rotation stellaires, lentilles gravitationnelles et mesures de satellites (Sagittarius, LMC). Même si leurs paramètres évoluent, le formalisme reste commun.

## Paramètres publiés dans le standard

- Masse du halo à 200 kpc : (1,3 ± 0,3) × 10¹² M☉  
- Profil recommandé : Einasto (α = 0,16 ± 0,02) pour compatibilité avec les simulations cosmologiques modernes.  
- Impact sur P : variation < 2 % entre les différents profils testés — valeur intégrée dans l’incertitude globale (section 1.4).

Chaque recalcul de l’année galactique doit documenter le profil de halo choisi. Les coefficients normalisés sont fournis dans `annexes/A2-formulaires-constantes.md` pour faciliter les implémentations logicielles.

