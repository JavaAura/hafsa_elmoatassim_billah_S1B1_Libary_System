# Bibliothèque Municipale - Application Console Java 8

## Description du Projet

Bienvenue dans le système de gestion informatisé de la bibliothèque municipale ! Cette application console, développée en Java 8, permet de gérer efficacement l'inventaire des livres et magazines, ainsi que les emprunts et retours. 
Ce projet vise à automatiser les tâches quotidiennes de la bibliothèque, offrant une solution moderne pour une gestion fluide et intuitive.

## UML

![UML](https://github.com/user-attachments/assets/7b8b046b-3930-44d3-9389-13abfbc3336e)

## Fonctionnalités Principales

- **Ajouter un document** : Ajoutez des livres et des magazines à l'inventaire.
- **Emprunter un document** : Gérez les emprunts de documents par les utilisateurs.
- **Retourner un document** : Suivez les retours de documents et mettez à jour l'inventaire.
- **Afficher tous les documents** : Visualisez l'ensemble des livres et magazines disponibles.
- **Rechercher un document** : Effectuez des recherches rapides par titre grâce à une implémentation HashMap.
- **Afficher La Liste des Documents Reservés** : Visualisez l'ensemble des livres et magazines reserves.
- **Quitter** : Fermez l'application en toute sécurité.

## Architecture du Projet

L'application est structurée selon une architecture en couches, offrant une séparation claire des responsabilités :

- **Couche de présentation** :
  - `ConsoleUI` : Gère l'interface utilisateur en console et les interactions avec l'utilisateur.

- **Couche métier** :
  - `Document` (Classe Abstraite) : Classe de base pour les livres et magazines, avec des méthodes abstraites pour les fonctionnalités essentielles.
  - `Livre` : Hérite de `Document` et ajoute un attribut spécifique (`isbn`).
  - `Magazine` : Hérite de `Document` et ajoute un attribut spécifique (`numero`).
  - `Bibliotheque` : Gère l'ensemble des documents et les opérations telles que l'ajout, l'emprunt, et la recherche.

- **Couche utilitaire** :
  - `DateUtils` : Fournit des méthodes pratiques pour la manipulation des dates, intégrant l'API Java Time.

## Spécifications Techniques

- **Stockage des documents** : Les documents sont stockés dans une `ArrayList` pour une gestion flexible.
- **Recherche rapide** : Implémentation d'une recherche rapide utilisant un `HashMap<String, Document>`.
- **Gestion des dates** : Utilisation de l'API Java Time pour une manipulation précise des dates.
- **Expressions Lambda** : Appliquées pour optimiser et simplifier certaines opérations.

## Instructions d'Installation

1. Clonez ce dépôt Git sur votre machine locale :
   ```bash
   git clone https://github.com/JavaAura/hafsa_elmoatassim_billah_S1B1_Libary_System
   ```

2. Assurez-vous d'avoir Java 8 installé sur votre machine.

3. Compilez et exécutez l'application depuis votre IDE préféré ou en ligne de commande :
   ```bash
   javac Main.java
   java Main
   ```

## Utilisation

À l'ouverture de l'application, un menu interactif s'affiche, vous permettant de choisir parmi les options disponibles :

```
Veuillez entrer votre choix (1-6) :
1. Ajouter un document
2. Emprunter un document
3. Retourner un document
4. Afficher tous les documents
5. Rechercher un document
6. Afficher La Liste des Documents Reservés
7. Quitter
```

## Gestion du Projet

- **Git** : Utilisé pour le contrôle de version.
- **JIRA** : Utilisé pour la gestion des tâches et le suivi des progrès.
- **Daily Stand-ups** : Simulations de réunions quotidiennes pour coordonner le travail et résoudre les obstacles.

## Contributions

Les contributions sont les bienvenues ! N'hésitez pas à faire un fork de ce dépôt et à soumettre vos pull requests.

## Auteurs

Ce projet a été réalisé par Hafsa Elmoatassim Billah dans le cadre d'un exercice de développement d'une application Java pour la gestion d'une bibliothèque municipale.
