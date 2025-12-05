# 2.5 — Microgalaces et nanogalaces

Pour les applications instrumentales (horloges atomiques, systèmes de contrôle, balises SUCL), le standard introduit :

- `1 microgalace (µG) = 10⁻¹⁵ GY ≈ 7,26 secondes`
- `1 nanogalace (nG) = 10⁻¹⁸ GY ≈ 7,26 millisecondes`

## Pourquoi descendre si bas ?

1. **Instrumentation scientifique** : les spectromètres, télémesures gravitationnelles et liaisons optiques nécessitent des résolutions de quelques secondes pour synchroniser des expériences réparties.
2. **Codage SUCL** : les séquences temporelles intégrées dans la Géode sont décrites en µG afin que l’ordre des événements reste clair même après des milliers d’années.
3. **Interopérabilité avec le SI** : la conversion `1 µG = 7,26 s` facilite l’alignement sur les horloges atomiques (césium, rubidium) déjà en place.

## Bonnes pratiques

- Limiter l’usage des µG aux documents techniques, afin de ne pas surcharger les récits destinés au grand public.
- Documenter la précision matérielle de l’oscillateur utilisé pour générer les µG.
- Éviter les subdivisions supplémentaires : au-delà du nanogalactique, il est préférable de revenir aux secondes SI.

Ces unités complètent la chaîne TG pour que chaque niveau, du cosmique au microsecondes, reste cohérent et traçable.

