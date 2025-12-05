# Chapitre 1 — Dynamique de la Voie lactée et année galactique

Ce premier chapitre établit la base astrophysique du Temps Galactique. Nous décrivons la morphologie spirale barrée de la Voie lactée, quantifions l’orbite solaire qui définit l’année galactique (GY), expliquons le rôle stabilisateur du halo de matière noire, puis détaillons les marges d’incertitude admises par le standard.

## Contenu des sections associées

- **1.1 Morphologie spirale barrée** : cartographie des bras (Persée, Sagittaire, Orion, Centaure) et de la barre centrale observable via radioastronomie.
- **1.2 Orbite solaire** : estimation du rayon galactocentrique, vitesse tangentielle, période moyenne et méthodes d’observation (Gaia, VLBI).
- **1.3 Halo sombre et stabilité** : contribution dynamique de la matière noire à la rotation quasi plate, justification du choix d’une période moyenne.
- **1.4 Variations et incertitudes** : effets des passages de bras, nuages moléculaires géants, erreurs de modèle ; tolérances officielles pour le GY.

Chaque fichier de section fournit les équations clés, des applications numériques et les recommandations de traçabilité nécessaires au reste du traité.

## Exemple mathématique concret

Calcul de la vitesse orbitale locale :

```
Θ(R) = √(G × M(<R) / R)
```

En insérant `M(<R) = 1,1×10¹¹ M☉` et `R = 8,178 kpc`, on obtient `Θ ≈ 228 km·s⁻¹`, valeur cohérente avec la section 1.2 et utilisée dans toutes les conversions TG.

## Tableau de classification des composantes

| Composante | Masse relative | Signature d’observation | Impact sur GY |
|------------|----------------|--------------------------|---------------|
| Bulbe | 10 % | infrarouge, vitesses radiales | Faible, surtout marées internes |
| Barre | 15 % | cartographie infrarouge | Définit l’orientation de R₀ |
| Disque mince | 20 % | H I 21 cm, Hα | Influence locale sur Θ |
| Halo sombre | 55 % | courbes de rotation, lentilles | Stabilise la période |

## Encadrés spéciaux

- ⚠️ **Attention** : utiliser une valeur obsolète de R₀ fausse toutes les conversions TG. Vérifiez la version `TG.vYYYY` avant publication.
- 💡 **Conseil** : associez toujours vos cartes à un jeu d’étoiles repères (pulsars, amas globulaires) pour faciliter la reconstitution future.
- ✓ **Bonnes pratiques** : documentez l’origine de chaque constante (mission Gaia, VLBI…) dans vos métadonnées SUCL.

## Synthèse & évaluation

- **À retenir** : l’année galactique dépend d’une combinaison bulbe+disque+halo ; aucune mesure isolée ne suffit.
- **Question rapide** : expliquer comment la présence du halo sombre limite les variations de vitesse lors du passage dans un bras spiral.

