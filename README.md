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
In spring , any object managed by the Spring IoC container
is called a "bean". These beans are typically defined in
configuration files(or using annotations) and are created 
and wired by spring according to the app needs.
In this project classes like "UserService" or "UserRepository" would
be configured as beans so that they can be injected where we need them.


### Bean Scopes
Bean scopes define the lifecycle and visibility of 
a bean inside the Spring application. some common scopes include:
 * Singleton: A single instance of the bean is created and shared across the entire app.
 * Prototype: A new instance is created every time the bean is requested.
 * Request: Creates a bean for a single HTTP request(useful for webapps).
 * Session: A bean instance is create for each user session.

Depending on the requirements of the User management system, you 
might choose a different scope for your beans.

### ApplicationContext
The ApplicationContext is the central interface to the Spring container,
providing configuration, managing beans, and handling dependencies.


### Component Scanning and Stereotype Annotations
Spring offers a feature called Component Scanning that 
automatically detects and registers beans in the application 
context based on annotations.

### Spring Data JPA
Spring Data JPA is a module that simplifies data access in Spring 
applications. It provides a set of interfaces and helper methods 
to interact with the database, making CRUD operations (Create, Read, Update, Delete) easy to implement.

### Spring MVC
Spring MVC (Model-View-Controller) is a web module within Spring 
that allows us to handle HTTP requests and responses.

### Installation and Setup
Setting up a Spring project without Spring Boot involves 
configuring dependencies and creating necessary configuration
files to define beans, specify dependency injection, and 
configure the MVC framework. This setup requires manual 
steps, such as adding the Spring libraries, setting up an 
ApplicationContext, and configuring XML or Java-based 
configurations for your beans.