# Gestion des employés d'une petite entreprise

Ce projet Java met en place un système de gestion hiérarchique des employés d'une petite entreprise avec une base de données MySQL. Il permet d'afficher les noms et salaires des employés du directeur général aux développeurs en suivant une hiérarchie définie.

## Structure hiérarchique

- **Directeur Général** : Au sommet de la hiérarchie.
- **Manager** : Sous la responsabilité du directeur général, gérant deux développeurs.
- **Développeurs** : Trois développeurs, deux sous le manager et un sous le directeur général.

## Fonctionnalités

- Connexion à une base de données MySQL pour la gestion des employés.
- Implémentation des opérations CRUD (Create, read, update, delete) pour les employés.
- Affichage des informations des employés de manière hiérarchique.

## Instructions d'installation

1. Création d'un fichier `base.properties` dans la racine du projet contenant les informations de connexion à la base de données :

    jdbc.driver=com.mysql.jdbc.Driver.
   
    jdbc.url=jdbc:mysql://localhost/entreprise
   
    jdbc.username=root
   
    jdbc.password=root
   

3. Compilation et exécution des classes Java pour tester la gestion des employés.

## Packages principaux

- **`ma.projet.connexion`** : Gère la connexion à la base de données.
- **`ma.projet.beans`** : Contient les classes `Personne`, `Manager`, et `Developpeur`.
- **`ma.projet.dao`** : Contient l'interface `IDao` pour la gestion des opérations sur les employés.
- **`ma.projet.service`** : Implémente les services de gestion des employés (`ManagerService`, `DeveloppeurService`).
- **`ma.projet.test`** : Contient la classe `Entreprise` pour tester les fonctionnalités du projet.

## les classes
- Personne
- Developpeur
- Manager
- Connexion
- IDao
- DeveloppeurServic
- ManagerService
- Entreprise
