# 4.1 — SUCL : concept et champs obligatoires

SUCL (Standard Universal Chrono-Lattice) est une grammaire temporelle inspirée de la structure hexagonale des ondes de densité galactiques. Chaque message SUCL comprend :

1. **Bloc Identité** : version TG (`TG.vXXXX`), checksum, référence au site émetteur.
2. **Bloc Temps** : séquence hiérarchique `GY > HÉL > COS > G > sG > µG`, avec incertitudes.
3. **Bloc Contexte** : orientation spatiale (vecteur vers Sagittarius A*, angle galactique) indispensable pour comprendre l’origine.
4. **Bloc Intention** : type de message (avertissement, archive, signal scientifique) codé sous forme iconique.

## Syntaxe

```
SUCL[
  ID{TG.v2025 | GEO-01 | CRC=…}
  TIME{GY 0 | HÉL 008.742 | COS 512 | G 37.42}
  SPACE{R0=8.178 kpc | Θ0=229 km/s}
  INTENT{WARN}
]
```

Les champs supplémentaires (langue, scripts, images) sont encapsulés via MULS (section 4.3). SUCL agit donc comme l’épine dorsale temporelle sur laquelle toutes les narrations peuvent se greffer.

