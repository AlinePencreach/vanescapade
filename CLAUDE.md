# Van Escapade — ECF Développeur Web et Web Mobile

Application de location de vans aménagés (agence fictive à Aix-en-Provence). Le sujet complet, avec toutes les règles de gestion, est dans `docs/SUJET-ECF.md` : le relire avant chaque nouvelle fonctionnalité.

## Stack

<!-- À compléter avant de commencer, par exemple : Laravel 11, Blade, MySQL 8, MongoDB (statistiques admin), Vite. -->

## Design (validé, ne pas réinventer)

Tout le design est dans `docs/design/` :
- `CHARTE.md` : palette, typographie, espacements, règles d'accessibilité (RGAA) et de contenu. À lire en premier.
- `tokens.css` : toutes les variables CSS (couleurs en thème clair/sombre, espacements, arrondis, ombres). Ne jamais écrire une couleur, une taille ou un espacement en dur : toujours `var(--…)`.
- `van-escapade.css` : les classes des composants (préfixe `ve-`). À reprendre tel quel dans `resources/css/` et à transformer en composants Blade (`<x-button>`, `<x-van-card>`, `<x-badge>`…).
- `composants/*.md` + `composants/*.html` : pour chaque composant, ses règles d'usage et un rendu de référence.
- `maquettes/*.html` : les 6 écrans de référence (accueil, catalogue, fiche van), en bureau (1280 px) et mobile (390 px). Les ouvrir dans un navigateur ; l'intégration doit y correspondre.
- `logos/` : logo (SVG) et favicons.

Les illustrations des maquettes sont des espaces réservés : en production, utiliser des photos WebP 4:3. Les écrans non maquettés (réservation, espaces utilisateur / employé / admin, contact, connexion) se construisent avec les mêmes composants et tokens.

## Règles de travail

- Git : `main`, `develop`, une branche `feature/…` par fonctionnalité, issue de `develop` et fusionnée dedans après test.
- Base de données : fichiers SQL écrits à la main (création + jeu de données) dans `database/sql/`, en plus des éventuelles migrations : le sujet l'exige.
- Sécurité : requêtes préparées, protection CSRF et XSS, mots de passe hachés, contrôle des rôles côté serveur, vérification des chevauchements de réservation côté serveur dans une transaction.
- Accessibilité : contrastes de la charte, focus visible, libellés de champs, zones cliquables de 44 px.
