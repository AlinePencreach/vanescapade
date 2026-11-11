Van Escapade loue des vans aménagés depuis Aix-en-Provence. L'interface doit donner envie de partir (voyage, aventure) tout en rassurant (sérénité) : un ton frais et direct, jamais enfantin. Le système suit les « Règles de design » : peu de valeurs, définies une fois dans `tokens.json`, réutilisées partout.

## Ton et contenu

- Vouvoiement, phrases courtes, vocabulaire concret : « Réserver ce van », « Retrait de 9 h à 12 h », « Caution non encaissée ».
- Les boutons commencent par un verbe d'action. Jamais « OK », « Valider » seul ou « Cliquez ici ».
- Format français partout : `1 068,25 €`, `12/07/2027`, `9 h – 12 h`, espace insécable avant `€`, `%`, `:`.
- Pas d'emoji, pas de points d'exclamation en série, pas de superlatifs creux (« incroyable », « le meilleur »). On montre plutôt les preuves : vans contrôlés, assistance 7 j/7, avis vérifiés.
- Les noms des vans viennent de la région (Le Ventoux, Calanque, Luberon, Sainte-Victoire, Camargue, Verdon).
- Les majuscules sont réservées au style `overline` (catégorie du van, sur-titres de section).

## Couleurs

La palette d'Aline, six teintes à l'esprit vanlife années 70 (mer, route, coucher de soleil), organisées en quatre familles et réparties 60-30-10 :

| Teinte | Hex | Famille / token | Rôle | Part |
| --- | --- | --- | --- | --- |
| Crème et sable | FAE4AA | `sable-*` (`sable-200`) | Fonds, bandeaux chauds, bandes rétro | ~60 % |
| Marine | 09425E | `marine-700` | Couleur de marque : boutons, liens, titres colorés, pied de page | ~30 % |
| Bleu | 106A97 | `marine-500` | Survol, information | |
| Ciel | 7EABBF | `marine-300` | Secondaire : arcs rétro, illustrations, fonds teintés | |
| Orange | FE6917 | `orange-500` | Accent : « van » du logo, soleil, étoiles, encart Conditions | ~10 % |
| Sapin | 326659 | `sapin-500` | Succès, forêts et montagnes des illustrations | |

- Les composants n'utilisent **que les rôles** : `bg` (crème), `surface`, `surface-sunken` (sable), `border`, `border-strong`, `ink` (encre marine #14232b, jamais de noir pur), `ink-muted`, `action` (marine) + `action-hover` (bleu), `on-action`, `action-soft`, `on-action-soft`, `accent` (orange) + `on-accent`, `accent-soft`, `on-accent-soft`, `focus`, et `success` (sapin) / `warning` / `error` / `info` (bleu), chacun en `-soft` et `-ink`.
- **Orange = décor, jamais de texte blanc dessus** : le blanc sur FE6917 ne fait que 2,9:1. Sur un fond orange, le texte est `on-accent` (encre marine). Le texte orangé lisible utilise `on-accent-soft` (`orange-800`). Les étoiles orange sont toujours doublées de la note en texte.
- Ciel et sable ne portent jamais de texte (2,5:1 et 1,25:1 sur blanc) : ce sont des fonds.
- Tous les couples texte/fond nommés dans les notes d'usage dépassent 4,5:1 dans les **deux thèmes** ; bordures de champ, icônes de statut et anneau de focus dépassent 3:1.
- La couleur n'est jamais seule porteuse de sens : statut = couleur + icône + libellé ; erreur = bordure + icône + message ; jour réservé = gris + barré.
- Thème sombre : fond marine très profond (`bg` #0b1a22), `action` en ciel clair avec texte marine dessus, « escapade » du logo en `sable-200`.

### Touche rétro

Le motif signature est le **coucher de soleil en arcs concentriques** (ciel, sable, orange clair, orange) et les **trois bandes** orange / orange clair / ciel sur la carrosserie des vans. À utiliser dans les illustrations, le hero et la couverture, jamais sur les composants d'interface.

## Typographie

L'interface utilise une seule famille, **Figtree** (Google Fonts, OFL) : titres, texte, boutons, prix. La hiérarchie vient de la taille, de la graisse (400 / 600 / 700) et de la couleur. Le logo est lui aussi en Figtree : une seule police pour toute la marque.

| Style | Taille / interligne | Graisse | Usage |
| --- | --- | --- | --- |
| `display` | 56 / 1,05 | 700 | Hero de l'accueil, bureau seulement |
| `h1` | 36 / 1,15 | 700 | Titre de page, grands titres de section |
| `h2` | 24 / 1,25 | 600 | Titres de bloc, encarts |
| `h3` | 20 / 1,3 | 600 | Nom du van sur une carte |
| `body` / `body-strong` | 16 / 1,5 | 400 / 600 | Texte courant, boutons, prix |
| `small` | 14 / 1,5 | 400 | Aides, métadonnées, pied de page |
| `caption` / `overline` | 12 / 1,4 | 500 / 600 | Badges, légendes, catégories en majuscules |

Sur mobile, le hero passe en `h1` et les titres de section en `h2`. Paragraphes à 50–75 caractères, alignés à gauche, jamais justifiés.

## Espacement, grille, arrondis, ombres

- Échelle unique base 4/8 : `space-xs` 4 · `space-sm` 8 · `space-md` 16 · `space-lg` 24 · `space-xl` 32 · `space-2xl` 64 · `space-3xl` 96. Rien d'autre.
- Grille bureau 12 colonnes, contenu 1 160 px, gouttière `space-lg` ; mobile 4 colonnes, marges `space-md`. Maquettes à 1 280 px et 390 px.
- Arrondis : `radius-sm` 6 (cases, jours du calendrier), `radius-md` 10 (boutons et champs, toujours le même dans un formulaire), `radius-lg` 18 (cartes, photos, encarts), `radius-full` (puces, badges, avatars). Généreux mais pas ronds : convivial, pas « jouet ».
- Ombres teintées marine, douces : `shadow-1` cartes, `shadow-2` survol et barre de recherche, `shadow-3` carte de réservation collante, `shadow-4` modales. Une carte a une ombre **ou** une bordure fine (`ve-card--flat`), jamais les deux.

## États et accessibilité (RGAA)

- Chaque composant interactif existe en défaut, survol, focus, actif, désactivé, chargement (et erreur pour les champs).
- Focus clavier unique : anneau `focus` plein de 3 px, décalé de 2 px, visible sur toutes les surfaces.
- Zones cliquables d'au moins 44 × 44 px sur mobile ; boutons et champs à 44 px de haut.
- Libellés toujours visibles au-dessus des champs ; erreurs reliées par `aria-describedby`.
- Filtres du catalogue : résultat annoncé dans une zone `aria-live="polite"`.
- Images : texte alternatif décrivant le van ; ratio fixe 4:3 (cartes) pour éviter les sauts de mise en page.

## Iconographie et images

- Une seule bibliothèque : **Lucide** (licence ISC), trait 2 px, tailles 16 / 20 / 24, couleur héritée (`currentColor`). Dans Laravel : `blade-lucide-icons`.
- Une icône qui porte un sens a un libellé visible ou un `aria-label`.
- **Logo** : uniquement typographique, « **van**escapade » en minuscules et en Figtree : « van » 700 orange, « escapade » 400 marine. Pas de pictogramme. Favicon : monogramme « ve » sur carré marine. Versions et règles dans la fiche **Logo** et le groupe d'assets **Logos** ; taille minimale 20 px de haut.
- Les illustrations des maquettes (paysage + silhouette de van à bandes rétro, en aplats de la palette) remplacent les photos. En production : photos WebP 4:3, même lumière chaude de fin de journée, exportées en 1x et 2x.

## Maquettes

Le groupe **Maquettes bureau** (1 280 px) et le groupe **Maquettes mobile** (390 px) contiennent les trois écrans clés demandés par l'ECF : Accueil, Catalogue avec filtres, Fiche van (conditions de location mises en évidence, calendrier, réservation). Ils sont construits uniquement avec les composants ci-dessus.

## Composants

Classes CSS préfixées `ve-` dans `components/bundle.css`, prévues pour devenir des composants Blade (`<x-button>`, `<x-van-card>`, `<x-badge status="confirmee">`…). Chaque composant a sa fiche (usage, données à fournir, à éviter).
