# PriceSummary

Détail du prix affiché avant validation : nuits en basse et haute saison, remise durée, options, frais de livraison, total et caution.

- **Fournir** : les lignes calculées côté serveur (même calcul que celui enregistré), avec pour chacune le détail en `sub` (prix unitaire × quantité, période).
- Remise en `success-ink` avec une coche ; total en `font-display` 24 px ; caution dans un bloc `surface-sunken` qui précise « non encaissée ».
- Montants alignés à droite en chiffres tabulaires, format français (« 1 068,25 € »).
