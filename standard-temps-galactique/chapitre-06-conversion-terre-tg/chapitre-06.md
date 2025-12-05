# Chapitre 6 — Méthodes de conversion Terre ↔ Temps Galactique

L’adoption d’un référentiel galactique ne supprime pas les calendriers existants. Ce chapitre fournit les équations, algorithmes et exemples nécessaires pour passer des dates terrestres (ISO, JD, secondes SI) aux coordonnées TG et inversement.

## Contenu des sections associées

- **6.1 Équations de base** : formules reliant secondes SI, jours juliens (JD) et unités TG.
- **6.2 Algorithmes logiciels** : pseudo-code de convertisseurs, gestion des arrondis.
- **6.3 Tables de correspondance historique** : jalons (J2000, adoption TG, HÉL +1).
- **6.4 Erreurs cumulatives et corrections** : prise en compte des dérives, publication des versions.
- **6.5 Cas d’usage** : signalisation scientifique, diplomatie, patrimoine.

Ces éléments assurent que l’écosystème TG reste compatible avec les systèmes opérationnels actuels.

## Exemple mathématique concret

Conversion d’une seconde UTC vers TG :

```
1 s = 1 / (GY_seconds) GY
    = 1 / (230 000 000 × 31 556 926) GY
    ≈ 1,38×10⁻¹⁷ GY = 0,0138 µG
```

Ainsi, une seconde terrestre équivaut à 1,38 % d’une microgalace.

## Tableau de classification des formats

| Format source | Résolution | Avantages | Précautions |
|---------------|------------|-----------|-------------|
| ISO 8601 | 1 s | Compatible systèmes d’info | gérer fuseaux |
| JD / MJD | 10⁻⁵ jour | Standard astronomique | nécessite JD₀ |
| TAI | 10⁻⁹ s | Horloges atomiques | pas de secondes intercalaires |
| UNIX epoch | 1 s | Informatique grand public | dépend du TZ |

## Encadrés spéciaux

- ⚠️ **Attention** : oubliez de retrancher les secondes intercalaires avant conversion entraîne des erreurs supérieures à 0,1 COS en quelques décennies.
- 💡 **Conseil** : stockez les résultats TG sous forme d’entiers (HÉL, COS, G…) plutôt qu’en flottants pour éviter les glissements.
- ✓ **Bonnes pratiques** : publiez vos outils de conversion en open source et accompagnez-les d’une suite de tests (voir A5).

## Synthèse & évaluation

- **À retenir** : la robustesse du TG dépend de la traçabilité de la chaîne de conversion.
- **Question rapide** : comment gérer un document produit sous `TG.v2025` lorsqu’une future `TG.v2050` modifie la valeur de GY ?

