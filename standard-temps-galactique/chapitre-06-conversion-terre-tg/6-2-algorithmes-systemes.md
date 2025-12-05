# 6.2 — Algorithmes logiciels et considérations systèmes

Cette section décrit l’algorithme de référence `TERRE→TG`, compatible avec des environnements embarqués ou cloud.

```
function terre_to_tg(date_iso):
    jd = iso_to_julian(date_iso)
    seconds = (jd - JD_EZG) * 86400
    frac = seconds / GY_SECONDS
    hel = floor(frac * 1e6)
    cos = floor(frac * 1e9) % 1000
    g   = floor(frac * 1e11) % 100
    sg  = floor(frac * 1e13) % 100
    mug = floor(frac * 1e15) % 100
    return {hel, cos, g, sg, mug}
```

## Points clés d’implémentation

- **Précision** : utiliser des flottants 128 bits ou des entiers arbitraires pour éviter la perte d’information lors des multiplications.
- **Fuseaux horaires** : convertir d’abord la date ISO vers UTC avant de basculer sur JD.
- **Versioning** : inclure dans chaque fonction un paramètre `tg_version`, afin de mettre à jour les constantes sans recompiler tout le logiciel.
- **Tests** : un jeu de cas (Annexe A5) permet de valider les implémentations en comparant les résultats à ±1 µG.

Des bibliothèques de référence (`tg-core`) seront publiées en open-source pour accélérer l’adoption.

