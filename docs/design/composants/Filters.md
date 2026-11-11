# Filters

Contrôles du catalogue : puces `ve-chip` (catégorie, couchages), curseur double `ve-range` (fourchette de prix ; un seul pouce = prix maximum), cases `ve-check` (équipements, avec le nombre de vans concernés) et radios (boîte de vitesses).

- **Fournir** : le libellé du groupe (`ve-label`, en `fieldset`/`legend` dans le code), les options, l'état coché.
- Les puces actives portent `aria-pressed="true"`, le fond `action-soft` **et** une coche : l'état ne repose pas sur la couleur.
- Les résultats se mettent à jour sans rechargement : annoncer le nouveau nombre dans une zone `aria-live="polite"` (« 4 vans correspondent »).
- Sur mobile, les filtres passent dans un panneau plein écran ouvert par « Filtres (n) » ; les filtres actifs restent visibles en puces au-dessus des résultats.
