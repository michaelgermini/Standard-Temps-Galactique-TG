# Annexe A4 — Norme ISO‑TG (extrait)

Cette annexe propose une structure inspirée des normes ISO pour décrire les implémentations du Temps Galactique.

## 1. Objet et domaine d’application

La norme ISO‑TG définit :

- Les formats de fichiers (`.tgdoc`, `.tgjson`).
- Les protocoles SUCL/MULS minimaux pour toute archive.
- Les algorithmes de conversion Terre ↔ TG (pseudo-code section 6.2).

## 2. Structure d’un fichier `.tgjson`

```json
{
  "tg_version": "TG.v2025",
  "ezg_offset": "-0.0001356",
  "time": {
    "hel": 8,
    "cos": 742,
    "g": 37,
    "sg": 42,
    "micro": 18
  },
  "uncertainty": 0.087,
  "context": {
    "r0_kpc": 8.178,
    "theta0_kms": 229,
    "space_ref": "Sagittarius A*"
  }
}
```

## 3. Gabarits SUCL

- Spirale logarithmique fournie en SVG (1 unité = 1 µG).
- Pictogrammes pour les champs `INTENT` (WARN, ARCHIVE, CELEBRATE).

## 4. Procédures de conformité

- Tests unitaires obligatoires sur les conversions (voir annexe A5).
- Audit indépendant avant publication d’une Géode ou d’un logiciel grand public.

Les institutions sont encouragées à soumettre leurs extensions à un registre public pour éviter les divergences.

