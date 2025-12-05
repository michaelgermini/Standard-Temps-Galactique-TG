# Chapitre 2 — Définition des unités du Temps Galactique

Après avoir fixé la dynamique orbitale, nous définissons une hiérarchie d’unités fondée sur la division décimale du GY. L’objectif : disposer d’unités adaptées aux récits cosmologiques, aux chronologies civilisationnelles et aux activités quotidiennes — tout en restant calculables à partir de la période orbitale.

## Contenu des sections associées

- **2.1 Année galactique (GY)** : unité fondamentale, équations de conversion, stockage des incertitudes.
- **2.2 Héliotique (HÉL)** : subdivision 10⁻⁶ du GY, pensée pour documenter l’histoire des civilisations.
- **2.3 Cycle d’Orbite Solaire (COS)** : 10⁻⁹ du GY (~84 jours terrestres), unité “mensuelle”.
- **2.4 Galace et sous-galaces** : 10⁻¹¹ et 10⁻¹³ du GY (≈20 h et 12 min), unités quotidiennes indépendantes des planètes.
- **2.5 Micro/Nano-galaces** : granularité opérationnelle (≈7 s) pour instrumentation scientifique.
- **2.6 Comparaison avec les unités terrestres** : tableaux de conversion, cas pratiques, recommandations logicielles.

Chaque fichier fournit la notation officielle, les préfixes autorisés, les exemples d’écriture SUCL et les implications culturelles de l’utilisation de ces unités.

## Exemple mathématique concret

Conversion d’une durée terrestre en unités TG :

```
Durée = 500 ans
HÉL = 500 / 230 = 2,1739
COS = 0,1739 × 1000 = 173,9 ≈ 174 COS
```

La durée de 500 ans correspond donc à `HÉL 002 + COS 174`, ce qui facilite la communication interplanétaire.

## Tableau de classification des unités

| Unité | Facteur vs GY | Durée terrestre | Domaine d’usage |
|-------|---------------|-----------------|-----------------|
| GY | 1 | 230 Myr | Cosmologie |
| HÉL | 10⁻⁶ | 230 ans | Politiques longues |
| COS | 10⁻⁹ | 84 jours | Planification opérationnelle |
| G | 10⁻¹¹ | 20 h | Rythme quotidien |
| sG | 10⁻¹³ | 12 min | Réunions, shifts |
| µG | 10⁻¹⁵ | 7,26 s | Instrumentation |

## Encadrés spéciaux

- ⚠️ **Attention** : n’utilisez pas de facteur binaire (base 2) pour subdiviser les unités TG ; cela casserait la compatibilité SUCL.
- 💡 **Conseil** : pour sensibiliser le public, présentez les COS comme des “quadrimestres galactiques” (≈84 jours), analogie simple et mémorable.
- ✓ **Bonnes pratiques** : incluez toujours l’incertitude relative (`±8,7 %`) lorsque vous annoncez une valeur en GY.

## Synthèse & évaluation

- **À retenir** : la hiérarchie décimale garantit que les unités s’emboîtent sans perte d’information.
- **Question rapide** : combien de galaces contient un HÉL ? (Réponse : 10⁶ galaces).

