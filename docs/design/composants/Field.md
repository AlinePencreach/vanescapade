# Field

Champ de formulaire complet : `ve-field` > `ve-label` + `ve-input` + `ve-help` ou `ve-error`.

- **Fournir** : un libellé toujours visible au-dessus (le placeholder n'est pas un libellé), le texte d'aide utile (format, contrainte), l'icône Lucide qui décrit la donnée.
- **Hauteur** : 44 px, comme les boutons, arrondi `radius-md` identique.
- **Erreur** : bordure `error` + message `ve-error` sous le champ, en `error-ink` avec l'icône `alert-circle` — jamais la couleur seule. Relier le message avec `aria-describedby` et poser `aria-invalid="true"`.
- **Désactivé** : `surface-sunken` + `ink-muted`, et un texte d'aide qui explique pourquoi (ex. le van ne peut pas être changé après réservation).
- Mot de passe : afficher la règle complète dès le départ, pas seulement en cas d'erreur.
