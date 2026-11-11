# Badge

Pastille courte (`ve-badge`, arrondi `radius-full`, texte `caption` 600) : fond clair + texte foncé de la même teinte, **toujours avec une icône**.

| Statut de réservation | Ton | Icône |
| --- | --- | --- |
| En attente | neutre | hourglass |
| Confirmée | `info` | check |
| En préparation | `primary` | wrench |
| Remis au client | `primary` | key |
| Retourné | neutre | undo |
| En attente de règlement | `warning` | euro |
| Clôturée | `success` | check |
| Annulée | `error` | x |

- Sur une photo, utiliser `ve-badge--solid` (fond `surface` + `shadow-1`) pour rester lisible.
- `ve-badge--accent` est réservé à « Coup de cœur » : un seul par écran.
