# Gestion des Employés 

## Description
Ce projet consiste en une application Java de gestion des employés d'une petite entreprise. L'entreprise est composée de cinq employés : un directeur général, un manager, et trois développeurs. L'objectif est de créer une structure hiérarchique et d'afficher les noms et les salaires des employés, du plus haut au plus bas niveau.

## Structure du Projet
Le projet est structuré autour de plusieurs packages Java :

- ma.projet.beans : contient les classes des entités Personne, Manager, et Developpeur.
- ma.projet.dao : contient l'interface IDao qui définit les méthodes CRUD (Create, Read, Update, Delete) pour les entités.
- ma.projet.service : contient les services ManagerService et DeveloppeurService qui implémentent l'interface IDao et gèrent les opérations de gestion des employés.
- ma.projet.test : contient la classe Entreprise pour tester les opérations CRUD et afficher les informations des employés.

## Partie I : Couche d'Accès aux Données

### Connexion à la Base de Données
- Un fichier base.properties est créé dans la racine du projet pour stocker les informations de connexion à la base de données MySQL.
- La classe Connexion permet d'établir la connexion à la base de données à l'aide des informations du fichier properties.

## Partie II : Implémentation des Entités

### Classes à Créer dans ma.projet.beans
- Personne : Représente une personne dans l'entreprise avec un identifiant, un nom, et un salaire.
- Manager : Hérite de Personne et gère une équipe de développeurs.
- Developpeur : Hérite de Personne et représente un développeur dans l'entreprise.

### Interface IDao
L'interface IDao dans le package ma.projet.dao fournit les méthodes CRUD pour les entités (création, mise à jour, suppression, récupération).

## Partie III : Services

### Services à Créer dans ma.projet.service
- ManagerService : Gère les managers.
- DeveloppeurService : Gère les développeurs.

## Partie IV : Tests

### Classe Entreprise
La classe Entreprise dans le package ma.projet.test permet de tester les opérations CRUD pour les employés et affiche les informations des employés par ordre hiérarchique.

## Installation et Exécution
