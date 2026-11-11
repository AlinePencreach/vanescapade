# Button

Bouton d'action en trois niveaux : `ve-btn--primary` (plein Lagon, une seule fois par zone), `ve-btn--secondary` (contour) et `ve-btn--tertiary` (texte seul).

- **Fournir** : un libellé qui commence par un verbe (« Réserver ce van », « Voir les dates », « Enregistrer mes informations ») — jamais « OK » ni « Valider » seul. Une icône Lucide 16–20 px optionnelle avant le libellé.
- **Tailles** : 44 px par défaut, `ve-btn--lg` 52 px (hero, barre de réservation mobile), `ve-btn--sm` 36 px (cartes, en-tête). `ve-btn--block` pour la pleine largeur sur mobile.
- **États** : survol `action-hover`, focus = anneau `focus` 3 px décalé de 2 px, désactivé `surface-sunken` + `ink-muted` + attribut `disabled`, chargement = spinner + libellé au présent progressif et `aria-busy="true"`.
- **À éviter** : deux boutons primaires côte à côte ; un bouton qui ressemble à un lien pour une action destructive (utiliser secondaire + modale de confirmation).

En Blade : `<x-button variant="primary" size="lg" icon="calendar">Réserver ce van</x-button>`.
