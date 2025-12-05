# 4.4 — Interopérabilité SUCL–MULS

SUCL fournit les coordonnées temporelles, tandis que MULS définit le médium. Pour garantir leur cohésion :

1. **Référencement croisé** : chaque paquet MULS inclut une section SUCL compressée. Inversement, les champs `INTENT` de SUCL pointent vers une couche MULS (`L3/data-id`).
2. **Checksums communs** : les hashages (SHA-512, BLAKE3) sont gravés à la fois dans SUCL (texte) et MULS (symboles). Toute divergence signale une corruption.
3. **Synchronisation des versions** : quand TG.vYYYY change, SUCL avertit via le champ `VER`, tandis que MULS précise comment, matériellement ou logiquement, appliquer la mise à jour.

## Exemple d’utilisation

- Un dépôt Git encode les commits critiques avec un en-tête SUCL. Les fichiers README décrivent les couches MULS (L3 : équations, L4 : récit).
- Une Géode physique grave SUCL sur son enveloppe externe (L1) ; les couches internes contiennent les disques MULS correspondant.

Cette interopérabilité assure que, quel que soit le mode d’accès (lecture optique, tactile, numérique), la chronologie reste alignée sur le standard TG.

