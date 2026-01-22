# Cahier des charges

Je pars de ce [tutoriel](https://blog.hubspot.fr/website/cahier-des-charges-application-mobile) pour créer le cahier des charges.

## Table des matières

1. [La présentation de l'entreprise](#1-la-présentation-de-lentreprise)
2. [L'objectif de l'application](#2-lobjectif-de-lapplication)
3. [La cible du projet](#3-la-cible-du-projet)
4. [Le périmètre du projet](#4-le-périmètre-du-projet)
5. [La charte graphique](#5-la-charte-graphique)
6. [La description du parcours utilisateur](#6-la-description-du-parcours-utilisateur)
7. [Les spécificités techniques et fonctionnelles](#7-les-spécificités-techniques-et-fonctionnelles)
8. [Les prestations attendues](#8-les-prestations-attendues)
9. [Le planning et les délais](#9-le-planning-et-les-délais)
10. [Le budget](#10-le-budget)

## 1. La présentation de l'entreprise

Ceci est un side project. Donc pas d'entreprise mise en jeu ici, mais une envie d'explorer comment créer une application web sécurisée pour accueillir quelques personnes en simultanée.

## 2. L'objectif de l'application

L'objectif est de créer une version open-source et navigateur du jeu **Shérif de Nottingham**, créé par Sergio Halaban, André Zatz et d'autres.

<p align="center">
<img src="./images/jeu.jpg" width=200 alt="Shérif de Nottingham">
<p align="center"><i>Shérif de Nottingham</i></p>
</p>

Strictement multijoueur de 4 à 5 personnes, avec des variantes pour 3 et 6 joueurs, chaque mode nécessite un développement légèrement différent.

2 versions du jeu existent, le développement ne concernera que la 2ème version (pour plus de facilité).

## 3. La cible du projet

Destiné à un public jouant aux jeux de société, ayant à disposition un canal vocal externe (e.g: Discord) et aimant l'aspect compétitif.

## 4. Le périmètre du projet

### a. Élements à respecter

#### i. Connexion au service

L'utilisateur **peut** se rendre sur l'URL de l'application. 

L'utilisateur **peut** se connecter via Oauth Google grâce au bouton *Connexion*.

**Optionnel**: Ajouter d'autres Oauth comme Facebook, Github, etc...

L'utilisateur **doit** choisir un pseudo à sa première connexion. Il peut le modifier à tout moment dans son *Profil* si aucun autre utilisateur n'a le même pseudo.

Une fois connecté, l'utilisateur **doit** être sur la *Page d'accueil*.

#### ii. Système de gestion d'amis

L'utilisateur **peut** ajouter des amis via une interface *Amis*.

L'utilisateur **peut** chercher d'autres utilisateurs via leur pseudo dans une interface *Recherche*.

L'utilisateur **peut** chercher parmi ses amis un autre utilisateur via une interface *Amis*.

L'utilisateur **peut** supprimer des amis via une interface *Amis*.

L'interface *Amis* doit être accessible à n'importe quel moment durant le parcours utilisateur. (surtout lors de [la création d'une partie](#ii-création-dune-partie))

#### iii. Création d'une partie

L'utilisateur **peut** cliquer sur le bouton *Nouvelle Partie* de la Navbar pour arriver sur l'interface de création de partie (Stepper).

L'utilisateur **doit** inviter des joueurs (nombre ∈ [ 3 ; 6 ]) dans le *Salon* de cette partie.

Dès que le nombre de joueur est valide (∈ [ 3 ; 6 ]), le bouton *Créer* devient cliquable.

L'utilisateur **peut** voir et accéder à ses parties en cours dans *Mes Parties*.

L'utilisateur **peut** voir l'historique (ou statistiques) de ses parties précédentes uniquement s'il active un *Toggle*.

**NB**: pour éviter une surcharge par un utilisateur en particulier, une limite sera imposée par utilisateur (une partie en simultanée seulement).

#### iv. Jouer à une partie

Lire les règles dans `docs/pdf/regles.pdf`.

Les règles font office de cahier des charges pour le déroulement d'une *Partie*.

#### iv. Déconnexion au service

L'utilisateur **peut** se déconnecter avec un bouton *Déconnexion* là où le bouton *Connexion*.

### b. Élements hors-périmètre

#### i. Système de Ligue

L'utilisateur **peut** créer une *Ligue* avec un groupe fixé d'amis. Il est *Administrateur* de cette *Ligue*.

L'*Administrateur* d'une *Ligue* **peut** créer une *Saison* en définissant un nombre de *Parties* à réaliser. Une fois les *Parties* réalisées, les statistiques d'une *Saison* sont accessibles aux participants.

L'*Administrateur* d'une *Ligue* **peut** supprimer une *Saison* en cours.

L'*Administrateur* d'une *Ligue* **peut** supprimer une *Ligue* en cours.

## 5. La charte graphique

font: BebasNeue

color: #496FE6 #A90708

## 6. La description du parcours utilisateur

## 7. Les spécificités techniques et fonctionnelles

## 8. Les prestations attendues

## 9. Le planning et les délais

## 10. Le budget

