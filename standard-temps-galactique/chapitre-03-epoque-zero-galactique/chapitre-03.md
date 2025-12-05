# Chapitre 3 — Origine commune : Époque Zéro Galactique (EZG)

Un calendrier n’existe que s’il se réfère à un point zéro partagé. L’Époque Zéro Galactique (EZG) fixe le moment où le plan orbital du Soleil a intersecté l’axe radial pointant vers Sagittarius A*. Cette référence géométrique reste valable quelle que soit la planète d’observation.

## Contenu des sections associées

- **3.1 Critères pour un point zéro** : exhaustivité scientifique, neutralité culturelle, reproductibilité.
- **3.2 Reconstruction géométrique** : méthodes de calcul rétrograde de l’orbite solaire.
- **3.3 Méthodes de datation** : outils astrochronologiques, radio-isotopes, modélisation numérique.
- **3.4 Normalisation et consensus** : processus de validation internationale, audits périodiques.
- **3.5 Implications archivistiques** : comment recalibrer les archives existantes et les sites de stockage longue durée.

Ce chapitre garantit que chaque institution qui adopte le TG puisse dater les événements passés et futurs sans ambiguïté.

## Exemple mathématique concret

Reconstruction de l’instant EZG :

```
θ(t) = θ₀ + ∫ (Θ(R(t))/R(t)) dt
```

En résolvant numériquement jusqu’à retrouver `θ(t) = 0`, on obtient `t = −31,2 Myr` (par rapport à 2025). Ce résultat devient l’offset utilisé dans toutes les dates TG.

## Tableau de classification des méthodes

| Méthode | Données requises | Résolution temporelle | Robustesse |
|---------|------------------|-----------------------|------------|
| Astrochronologie | Gaia, VLBI | ±0,5 Myr | Élevée |
| Isotopes ⁶⁰Fe | Carottes sédimentaires | ±1 Myr | Moyenne |
| Modèles paléoclimatiques | Archives géologiques | ±2 Myr | Complément |
| Simulations N-corps | Supercalculateurs | dépend du modèle | Validation |

## Encadrés spéciaux

- ⚠️ **Attention** : l’EZG ne doit pas être confondu avec l’année 0 des calendriers civils. Ne mélangez jamais les référentiels.
- 💡 **Conseil** : publiez vos scripts d’intégration (ou leurs checksums) dans les Géodes pour permettre la vérification future.
- ✓ **Bonnes pratiques** : stockez les métadonnées `EZG_METHOD` et `EZG_UNC` avec chaque archive longue durée.

## Synthèse & évaluation

- **À retenir** : l’EZG repose sur un événement géométrique observable, pas sur une convention politique.
- **Question rapide** : citez deux raisons pour lesquelles on combine isotopes et astrométrie dans la datation EZG.

