# VanCard

Carte d'un van dans le catalogue et sur l'accueil : photo 4:3, catégorie en `overline`, nom en `h3`, couchages / places / boîte, prix « à partir de » et bouton.

- **Fournir** : photo principale (WebP, ratio 4:3, texte alternatif « Photo du van <nom> »), nom, catégorie, couchages, places, boîte, prix journalier basse saison, étiquette optionnelle.
- Toute la carte est un lien vers la fiche ; le bouton n'est qu'un repère visuel (pas deux cibles différentes).
- Survol : `shadow-2` + montée de 2 px. Hors service : photo désaturée, badge `warning` « Hors service », bouton désactivé « Indisponible ».
- Grille : 3 colonnes en bureau (gouttière `space-lg`), 1 colonne en mobile.
