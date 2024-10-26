## SPRING FRAMEWORK

This application is a basic User Management System
built using Spring Core without Spring Boot,
Spring MVC, and Spring Data JPA. It allows users to perform CRUD operations
such as creating, viewing, updating, and deleting users through a web interface.

## Table of Contents
- [Project Structure](#project-structure)
- [Dependency Injection (DI)](#dependency-injection-di)
- [Inversion of Control (IoC)](#inversion-of-control-ioc)
- [Spring Beans](#spring-beans)
- [Bean Scopes](#bean-scopes)
- [ApplicationContext](#applicationcontext)
- [Component Scanning and Stereotype Annotations](#component-scanning-and-stereotype-annotations)
- [Spring Data JPA](#spring-data-jpa)
- [Spring MVC](#spring-mvc)
- [Installation and Setup](#installation-and-setup)

### Project Structure
In this spring app, the project is organized in a way that separates
different functionalities, making it easier to manage and develop.
The structure of this project is presented as the following :
```
Maska-master [spring-framework]
├── .idea
├── .smarttomcat
├── src
│   ├── main
│   │   ├── java
│   │   │   └── org.example
│   │   │       ├── controller
│   │   │       ├── model
│   │   │       ├── repository
│   │   │       ├── services
│   │   │       └── Main.java
│   │   └── webapp
│   │       └── WEB-INF
│   │           ├── views
│   │           ├── applicationContext.xml
│   │           ├── dispatcher-servlet.xml
│   │           └── web.xml
├── postgresql.yml
├── target
├── .gitignore
├── pom.xml
└── README.md
```
### Dependency Injection (DI)
L'injection de dépendances est un concept dans Spring, où le framework fournit les objets nécessaires à l'application plutôt que de les créer directement. Cela aide à réduire le couplage entre les parties de l'application, facilitant les tests et la maintenance.

### Inversion of Control (IoC)
L'inversion de contrôle (IoC) est un principe où le contrôle de la création et de la gestion des objets est confié au framework Spring. L'IoC gère la création des objets, la gestion des dépendances, et le cycle de vie des objets, permettant aux développeurs de se concentrer sur la logique de l'application.

### Spring Beans
Dans Spring, tout objet géré par le conteneur IoC est appelé un "bean". Ces beans sont définis dans des fichiers de configuration (ou avec des annotations) et sont créés et connectés par Spring selon les besoins de l'application. Dans ce projet, des classes comme "UserService" ou "UserRepository" seront configurées comme beans pour être injectées là où on en a besoin.

### Bean Scopes
Les portées des beans définissent le cycle de vie et la visibilité d'un bean dans l'application Spring. Quelques portées courantes incluent :
 * Singleton : Un seul bean est créé et partagé dans toute l'application.
 * Prototype : Un nouvel objet est créé chaque fois que le bean est demandé.
 * Request : Crée un bean pour chaque requête HTTP (utile pour les applications web).
 * Session : Un bean est créé pour chaque session utilisateur.

### ApplicationContext
L'ApplicationContext est l'interface centrale du conteneur Spring. Elle fournit la configuration, gère les beans et les dépendances.

### Component Scanning and Stereotype Annotations
Spring propose une fonctionnalité appelée "Scan de Composants" qui détecte et enregistre automatiquement les 
beans dans le contexte de l'application en fonction des annotations.

### Spring Data JPA
Spring Data JPA est un module qui simplifie l'accès aux données dans les applications Spring. Il fournit des interfaces et des méthodes pour interagir avec la base de données, facilitant les opérations CRUD (Create, Read, Update, Delete).

### Spring MVC
Spring MVC (Model-View-Controller) est un module web dans Spring qui permet de gérer les requêtes et les réponses HTTP.

### Installation and Setup
Pour configurer un projet Spring sans Spring Boot, il faut ajouter les dépendances et créer les fichiers de configuration pour définir les beans, gérer l'injection de dépendances, et configurer le framework MVC.