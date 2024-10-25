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
Dependency Infection is a concept in Spring,where the 
framework provides objects needed by the application rather than 
creating them itself. this is helpful because it louses the coupling 
between the app parts, allowing for easier testing and maintenance.

### Inversion of Control (IoC)
Inversion of Control (IoC) is a principle where the control 
of creating and managing objects is transferred from the program
to the spring framework. the IoC also takes care of objects
creation , dependency management, and the life cycle of objects.
this allows us the developers to focus more on the app logic rather than
worrying about objects management.

### Spring Beans

### Bean Scopes

### ApplicationContext

### Component Scanning and Stereotype Annotations

### Spring Data JPA

### Spring MVC

### Installation and Setup