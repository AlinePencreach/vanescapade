ECF d'entraînement – Van Escapade
11 nov. 2026 · @Aline
TP Développeur Web et Web Mobile — sujet d'entraînement (entreprise et personnes fictives, sujet construit sur le modèle de l'ECF « Vite & Gourmand »)
Durée indicative : 70 h · Documents autorisés : annexes · Matériel autorisé : calculatrice, tableur, etc.
Mettez-vous en situation d'examen : lisez tout le sujet avant de commencer, puis répondez en situation professionnelle aux besoins et problématiques exposés.
Compétences du référentiel concernées
Toutes les compétences du titre professionnel Développeur Web et Web Mobile sont évaluées à travers ce projet.
Activité type 1 — Développer la partie front-end d'une application web ou web mobile sécurisée
• Installer et configurer son environnement de travail en fonction du projet
• Maquetter des interfaces utilisateur web ou web mobile
• Réaliser des interfaces utilisateur statiques web ou web mobile
• Développer la partie dynamique des interfaces utilisateur web ou web mobile
Activité type 2 — Développer la partie back-end d'une application web ou web mobile sécurisée
• Mettre en place une base de données relationnelle
• Développer des composants d'accès aux données SQL et NoSQL
• Développer des composants métier côté serveur
• Documenter le déploiement d'une application dynamique web ou web mobile
Présentation de l'entreprise
« Van Escapade » est une petite agence de location de vans aménagés installée à Aix-en-Provence depuis 8 ans. Elle est tenue par Margaux et Karim, qui gèrent une flotte d'une dizaine de véhicules (fourgons aménagés, vans compacts, camping-cars profilés) loués à la journée ou à la semaine, principalement d'avril à octobre.
Aujourd'hui, les réservations se font par téléphone et sont notées dans un agenda papier. Résultat : des doubles réservations, des clients qui ne voient pas les conditions de location, et beaucoup de temps perdu au téléphone. Karim souhaite une application web qui présente la flotte, permette de réserver en ligne et facilite le suivi des locations par l'équipe.
Ni Margaux ni Karim n'ont de compétences en informatique : ils ont fait appel à l'agence CodeLine, connue pour livrer des projets de qualité dans des délais courts. Fraîchement diplômé(e), vous venez d'être embauché(e) chez CodeLine et vous êtes missionné(e) sur ce projet.
Le but de l'application est de présenter les vans aux visiteurs et de permettre la réservation en ligne, puis de suivre chaque location de la remise des clés jusqu'à la clôture.
Description du projet
Vous travaillez sous la direction du chef de projet, qui a recueilli les besoins suivants.
Page d'accueil
La page d'accueil doit comporter :
• Une présentation de l'agence et de son histoire
• La mise en avant de ses engagements (vans entretenus et contrôlés avant chaque départ, assistance 7j/7 pendant la location, conseils d'itinéraires)
• Les avis clients validés par l'équipe
Menu de l'application
Le menu doit comporter au minimum :
• Un retour vers la page d'accueil
• L'accès au catalogue de tous les vans
• La connexion (réservée aux utilisateurs, employés et administrateur). Vous pouvez créer d'autres catégories si vous les jugez nécessaires, en respectant les aspects réglementaires (RGPD et sécurité).
• L'accès à la page de contact
Pied de page
Les horaires d'ouverture de l'agence (retrait et retour des vans) doivent être visibles dans le pied de page, du lundi au dimanche. Un lien vers les mentions légales et vers les conditions générales de location (CGL) doit être proposé.
Catalogue des vans (vue globale)
Une vue globale présente de manière simple et récapitulative tous les vans proposés à la location. Les vans sont configurables depuis l'espace « Administrateur » et l'espace « Employé ». Un van dispose des caractéristiques suivantes :
• Un nom (ex. « Le Ventoux », « Calanque »)
• Une galerie d'images (extérieur et intérieur)
• Une description
• Une catégorie : fourgon aménagé, van compact, camping-car profilé (vous pouvez enrichir cette liste)
• La marque et le modèle du véhicule
• Le nombre de places assises (carte grise) et le nombre de couchages
• Le type de boîte de vitesses (manuelle ou automatique) et le carburant
• Une liste d'équipements (douche, WC chimique, chauffage stationnaire, panneau solaire, réfrigérateur, auvent…) : un même équipement peut être présent dans plusieurs vans
• Le tarif journalier en basse saison
• La durée minimale de location (ex. 3 nuits minimum)
• Les conditions de location propres au van (kilométrage inclus par jour, montant de la caution, âge minimum du conducteur, ancienneté minimale du permis, animaux acceptés ou non…)
• Un statut de disponibilité : un van peut être mis « hors service » (entretien, réparation) et ne plus être réservable
Par ailleurs, l'agence propose des options payantes communes à tous les vans (kit vaisselle, linge de lit, porte-vélos, chaise et table de camping, forfait ménage…). Chaque option a un nom, une description et un prix, soit par jour, soit forfaitaire.
La vue globale affiche pour chaque van : sa photo principale, son nom, sa catégorie, son nombre de couchages et son tarif journalier « à partir de », avec un bouton pour voir le détail. Cette vue est accessible aux personnes authentifiées comme non authentifiées.
Des filtres permettent une recherche rapide :
• Filtre par prix journalier maximum
• Filtre sur une fourchette de prix journalier
• Filtre par catégorie
• Filtre par nombre de couchages minimum
• Filtre par type de boîte de vitesses
• Filtre par équipement (ex. « avec douche »)
• Filtre par disponibilité sur une période (date de départ et date de retour) : seuls les vans libres sur toute la période sont affichés
Les résultats doivent se mettre à jour dynamiquement, sans rechargement de la page.
Création de compte
Un visiteur peut créer un compte en renseignant :
• Son nom et son prénom
• Son numéro de téléphone portable
• Son adresse mail et son adresse postale
• Sa date de naissance et la date d'obtention de son permis B
• Un mot de passe sécurisé (10 caractères minimum, dont au moins un caractère spécial, une majuscule, une minuscule et un chiffre)
À la création, le compte reçoit le rôle « utilisateur ». Un mail de bienvenue est envoyé automatiquement.
Connexion
L'utilisateur se connecte avec son adresse mail et son mot de passe. En cas d'oubli, un bouton « Mot de passe oublié » lui permet de saisir son adresse mail pour recevoir un lien de réinitialisation.
Vue détaillée d'un van
Au clic sur le bouton d'un van dans le catalogue, toutes ses informations doivent être visibles : toutes les données enregistrées en base doivent apparaître.
La vue détaillée affiche également un calendrier des disponibilités du van (jours déjà réservés ou bloqués pour entretien).
Un bouton « Réserver » redirige l'utilisateur authentifié vers la page de réservation, avec le van déjà sélectionné. Un visiteur non authentifié est invité à se connecter ou à créer un compte avant d'accéder à la réservation.
Attention : les conditions de location du van (caution, kilométrage inclus, âge et ancienneté de permis requis, durée minimale) doivent être mises bien en évidence, afin qu'aucun client ne puisse dire qu'il ne les a pas vues.
Réservation d'un van
Depuis la vue détaillée, le bouton « Réserver » mène au formulaire de réservation, qui demande :
• Le nom, le prénom, le mail et le téléphone du client (pré-remplis depuis le compte)
• La date et l'heure de retrait, la date et l'heure de retour (créneaux possibles : 9 h – 12 h et 14 h – 18 h, dans les horaires d'ouverture)
• Le lieu de retrait : à l'agence (gratuit) ou livraison à une adresse (15 € majorés de 0,80 € par kilomètre, aller-retour, si l'adresse n'est pas à Aix-en-Provence ; le même montant s'applique pour la reprise du van)
• Le van choisi (pré-sélectionné si le client vient de la vue détaillée)
• Les options souhaitées
Règles de gestion à respecter :
• La durée de location doit être au moins égale à la durée minimale du van.
• Un van ne peut pas être réservé sur une période qui chevauche une réservation existante (non annulée) ou un blocage pour entretien. Cette vérification doit être faite côté serveur, y compris si deux clients valident en même temps.
• Le conducteur doit respecter l'âge minimum et l'ancienneté de permis du van (calculés à partir des informations du compte).
• Haute saison (du 1er juillet au 31 août) : le tarif journalier est majoré de 30 % pour chaque jour compris dans cette période.
• Remise durée : -10 % sur le prix de la location (hors options et hors livraison) à partir de 7 nuits, -15 % à partir de 14 nuits.
Avant validation, un récapitulatif détaillé du prix est affiché : nombre de jours en basse et en haute saison, prix de la location, remise appliquée, options, frais de livraison, total, ainsi que le montant de la caution (non encaissée). Après validation, le client reçoit un mail de confirmation.
Espace utilisateur
Depuis son espace, l'utilisateur peut :
• Consulter le détail de toutes ses réservations
• Modifier ses informations personnelles
• Déposer une copie de son permis de conduire (PDF, JPG ou PNG, 2 Mo maximum) — ce fichier contient des données personnelles : précisez dans votre copie comment vous le stockez et le protégez
Une réservation peut être modifiée ou annulée tant qu'un employé ne l'a pas passée au statut « confirmée ». Tout est modifiable sauf le van choisi.
Une fois la réservation confirmée, l'utilisateur a accès à son suivi : la liste de tous les statuts par lesquels elle est passée, avec la date et l'heure de chaque changement.
Quand la réservation est « clôturée », l'utilisateur reçoit un mail l'invitant à se connecter pour laisser un avis depuis sa réservation : une note de 1 à 5 suivie d'un commentaire.
Espace employé
Après connexion, un employé accède à son espace. Il peut :
• Créer, modifier et supprimer les vans, les équipements, les options et les horaires
• Bloquer des périodes d'indisponibilité pour un van (entretien, contrôle technique)
• Valider ou refuser les avis clients, afin qu'ils apparaissent ou non sur la page d'accueil
Un employé ne peut modifier ou annuler une réservation qu'après avoir contacté le client par téléphone ou par mail : il doit alors saisir le mode de contact utilisé et le motif.
Un filtre permet de retrouver rapidement les réservations par statut, par van, par période ou par client.
L'employé fait évoluer les réservations selon les statuts suivants :
• « confirmée » : la réservation est validée par l'équipe
• « en préparation » : le van est nettoyé, contrôlé et équipé des options choisies
• « remis au client » : les clés ont été remises ; l'employé saisit le kilométrage et le niveau de carburant au départ
• « retourné » : le van est revenu ; l'employé saisit le kilométrage et le niveau de carburant au retour
• « en attente de règlement » : à l'état des lieux, des frais supplémentaires sont constatés (kilomètres au-delà du forfait facturés 0,35 € / km, plein non fait facturé 2,50 € / litre manquant, dommages éventuels avec description). Le client reçoit un mail détaillant les frais et l'informant que, faute de règlement sous 15 jours, la somme sera retenue sur sa caution (conformément aux CGL).
• « clôturée » : soit directement après « retourné » si aucun frais n'est dû, soit une fois les frais réglés
Le calcul des kilomètres supplémentaires (kilométrage inclus par jour × nombre de jours, comparé aux kilomètres réellement parcourus) doit être fait automatiquement par l'application.
Espace administrateur
Après connexion, l'administrateur accède à son espace. Il peut créer un compte « employé » en renseignant un mail (qui sert d'identifiant) et un mot de passe. L'employé reçoit un mail l'informant de la création de son compte, sans que le mot de passe y figure : il devra le demander à l'administrateur.
L'administrateur peut aussi désactiver un compte employé (départ de l'agence, par exemple). Karim précise que vous devez lui créer ce compte administrateur vous-même et qu'il ne doit pas être possible de créer un compte administrateur depuis l'application.
L'administrateur peut faire tout ce que fait un employé. En plus, il dispose de statistiques :
• Le nombre de réservations par van, comparable entre les vans via un graphique
• Le taux d'occupation de chaque van par mois (nombre de jours loués / nombre de jours du mois)
• Le chiffre d'affaires par van, avec un filtre par van et un filtre sur une période
Ces statistiques doivent être alimentées par une base de données non relationnelle.
Contact
Un visiteur peut contacter l'agence depuis la page contact accessible dans le menu. Le formulaire demande un titre, une description et son adresse mail pour obtenir une réponse. La demande est envoyée par mail à l'agence.
Déploiement et accessibilité
Le chef de projet conclut que le client exige le déploiement de l'application : des pénalités seront appliquées si elle n'est pas en ligne et fonctionnelle au moment de la livraison. L'application doit également être accessible, conformément au RGAA.
Annexe 1 : pistes pour la base de données
Contrairement à l'ECF d'origine, aucun MCD n'est fourni : sa conception fait partie de l'exercice. À titre indicatif, votre modèle devrait au minimum couvrir les notions suivantes :
• Utilisateur et rôle
• Van, catégorie, image, équipement (relation plusieurs-à-plusieurs avec le van)
• Option (et son lien avec la réservation, avec la quantité ou le nombre de jours)
• Réservation et historique des statuts (statut, date et heure, employé ayant fait le changement)
• Indisponibilité d'un van (date de début, date de fin, motif)
• État des lieux (kilométrage et carburant au départ et au retour, frais constatés)
• Avis (note, commentaire, statut de validation)
• Horaires d'ouverture
• Saison tarifaire (si vous choisissez de rendre les périodes de haute saison paramétrables plutôt que codées en dur — à justifier)
Fournissez un jeu de données de démonstration d'au moins 6 vans (dont un hors service), 8 options, 2 employés et des réservations couvrant tous les statuts.
Stack technique
Aucune technologie n'est imposée, à l'exception de l'utilisation d'une base de données relationnelle et d'une base de données non relationnelle.
Exemple de stack possible :
• Front : HTML5, CSS (Bootstrap ou Tailwind), JavaScript
• Back-end : PHP avec PDO, ou un framework (Symfony, Laravel)
• Base de données relationnelle : MySQL, MariaDB ou PostgreSQL
• Base de données NoSQL : MongoDB
• Déploiement : fly.io, Heroku, Azure, Vercel, un VPS…
Objectif et livrables
L'objectif de cet ECF est de passer par chaque étape de l'élaboration d'une solution de qualité : analyse des besoins, maquettage, intégration, développement des règles de gestion et déploiement.
Vous détaillerez dans votre copie les dispositions prises, notamment en matière de sécurité (authentification, gestion des rôles, protection contre les injections SQL, XSS et CSRF, stockage des fichiers déposés, gestion des réservations concurrentes). Vous devrez justifier tous vos choix techniques et exposer votre point de vue sur les technologies envisagées.
Les livrables attendus sont les suivants :
• Le lien du (ou des) dépôt(s) GitHub public(s) contenant le code de l'application
• Le lien de l'application déployée
• Le lien vers votre outil de gestion de projet (Jira, Notion, Trello…)
Le dépôt Git devra comporter :
• Un fichier README.md expliquant comment installer et lancer l'application en local
• Les bonnes pratiques Git :
    ◦ une branche principale
    ◦ une branche de développement
    ◦ une branche par fonctionnalité, issue de la branche de développement, fusionnée vers celle-ci après test
    ◦ une fusion de la branche de développement vers la branche principale une fois celle-ci correctement testée
• Les fichiers de création de la base de données et d'insertion des données, au format SQL (l'utilisation de fixtures ou de migrations ne prouve pas que vous maîtrisez le SQL)
• Un manuel d'utilisation au format PDF, présentant l'application et fournissant les identifiants permettant de tester les différents parcours (visiteur, utilisateur, employé, administrateur)
• Une charte graphique au format PDF :
    ◦ la palette de couleurs et les polices utilisées
    ◦ l'export des maquettes (wireframes et mockups) : 3 maquettes bureau et 3 maquettes mobile
• Une documentation de gestion de projet, expliquant votre organisation
• Une documentation technique :
    ◦ réflexions technologiques initiales sur le sujet
    ◦ configuration de votre environnement de travail
    ◦ modèle conceptuel de données (ou diagramme de classes)
    ◦ diagramme de cas d'utilisation et diagramme de séquence (par exemple : la réservation d'un van avec vérification de disponibilité)
    ◦ documentation du déploiement, expliquant votre démarche et ses différentes étapes
Récapitulatif des règles de gestion
Règle
Valeur
Mot de passe
10 caractères min., 1 majuscule, 1 minuscule, 1 chiffre, 1 caractère spécial
Durée minimale
Définie par van (ex. 3 nuits)
Haute saison
Du 1er juillet au 31 août, +30 % sur le tarif journalier
Remise durée
-10 % dès 7 nuits, -15 % dès 14 nuits (hors options et livraison)
Livraison hors Aix
15 € + 0,80 € / km aller-retour, à l'aller et au retour
Kilomètres supplémentaires
0,35 € / km au-delà du forfait inclus
Carburant manquant
2,50 € / litre
Délai de règlement des frais
15 jours, sinon retenue sur la caution
Modification / annulation client
Possible tant que la réservation n'est pas « confirmée » ; le van ne peut pas être changé
Compte administrateur
Créé par le développeur, jamais depuis l'application
Statistiques admin
Issues de la base NoSQL