# AvailabilityCalendar

Calendrier des disponibilités d'un van (fiche van) et sélecteur de dates (réservation).

- **Fournir** : le mois, les jours réservés (réservations non annulées), les jours bloqués pour entretien, la sélection en cours.
- Chaque état a deux indices visuels : réservé = gris **barré**, entretien = **hachures** + barré, séjour = plein Lagon, haute saison = trait Couchant sous le jour. Chaque jour porte un `aria-label` complet (« 12 juin, réservé »).
- Deux mois côte à côte en bureau, un seul en mobile avec flèches précédent / suivant (44 px de zone cliquable).
