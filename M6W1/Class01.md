# SpringBoot

## Introduction to SpringBoot
***Basically it's an open source framework designed to facilitate the creation of Java-based applications.***

**First question: What is Spring?**

It's a project Eco-System, which makes to program in Java more easier, fast and secure to the community. 

**Principal Sub-projects:**

**SpringBoot:** It's a Sub-Project of Spring that simplifies the creation process of applications based on Spring. It allows a default configuration to start new Spring projects faster without the need of extended manual configurations.

**SpringData:** It allows an easier coding to the access of data in different data warehouses including relational data base and not relational. The objective is to facilitate the implementation of repositories and data services.

**SpringCloud:** Is a set of tools to create distributed systems and micro-services based applications. It allows solutions to the distributed settings, service discovery, circuit breakers, load balancing and more...

**SpringSecurity:** It's an authentication framework and a access control to Spring based applications. It allows protection to common attacks, such as: Impersonation (CSRF), brute force attacks, and more. Ensuring that the applications are secure.

**SpringBatch:** It allows a robust solution to the batch processing. Ideal to develop applications that manage with large volumes of data, like data migrations and transaction processing.

**SpringWebServices:** It allows the creation of web services of contract first and the interoperability of SOAP Web Services. It allows the endpoint creations and SOAP clients in a efficient and easy way.

## What is NOT SpringBoot?

SpringBoot is not a Spring framework replacement. It is based on this framework to allow a set of libraries and API's that facilitated a lot the Spring develop

## SpringBoot Starter

An starter in SpringBoot is a dependency preconfigured which simplifies the addition of certain functionalities to the Spring applications. This starters contain a set of automatic dependencies that are designed to work together and allow an specific functionality, this dependencies are imported in a **"pom.xml"** file and it is structured like this: 

* pom.xml:
* starter A
* starter B
* starter C

### Web Starter

* **Spring-boot-starter-web:** This includes all the necesary dependencies to develop web applications, including Spring MVC, Tomcat as a embedded server.

## What is a annotation in Java?

* An annotation is a metadata form that allows data over a program but it's not part of the program. The annotations in Java doesn't affect directly the operation of the applied code.

* Are used to allow information to the tools and libraries that will be executed at compile time, deployment time and execution time.

### Initial annotations

* **@SpringBootConfiguration:** Is an annotation in Spring Boot that marks a class as the main source of configuration for a Spring Boot application.

* **@EnableAutoConfiguration:** Is a Spring Boot annotation that automatically configures your application based on the dependencies present in the classpath.

* **@ComponentScan:** Is a Spring annotation that tells Spring where to look for components, configurations, and services to automatically register them as beans.

## Bean

A "bean" is an object that is managed by the Inversion of Control container (IoC), beans are the central components in a Spring application that represents objects that are created, cofigured and assembled between the Spring container.

### Bean features

* Management and automatically creation
* Dependency injection 
* Controled life cicle 

### How to define a Bean 

* Using @Component annotation
* Using @Bean annotation in a configuration class

## Spring MVC
***Model, View and Controller***

Is a framework within Spring that follows the Model-View-Controller (MVC) pattern to build web applications by separating the business logic, user interface, and control flow.

### Spring MVC Flow
![alt text](image.png)

### Spring MVC Layers

####  Presentation Layer(Controller, View, Model)
* **Controller:** Manages the user requests, interacts with the Business Layer and selects the proper view to return to the user. Acts like an intermediary between the view and the model.
* **View:** Is responsible to show the data to the user.
* **Model:** It represents the application data and the business logic. En Spring MVC it normally is POJO objects(Plain Old Java Object), that contains data and methods to manipulate this data.

#### Business Layer(Service)
***Here it is where it's implemented the rules and specific process of the domain of the App.***
* **@Service:** The @Service annotation it is used to mark a class like a service component. 

#### Access Layer(repository)
***This layer is the responsible to interact with the data base or any other file storage. Includes the logic to obtain, store and manipulate data.***
* **@Repository:** It can be used to mark a class like a data access component.
* This layer its in charge of the CRUD operations in the data base.

### Spring MVC graphic
![alt text](image-1.png)

## Stereotype
***Are annotations that are used to indicate the role of a component in the architecture of the application.***

This annotations not only mark a class like a Bean(that is managed by the Spring container), it also gave additional information about the purpose and functionality of the Bean.

### Most Common stereotypes
* @Component
* @Service
* @Repository
* @Controller

Spring defines several stereotypes that are essential for proper functioning and organization of an app.

This stereotypes helps Spring to detect automatically and configure beans inside the Spring container.

## To search...
* **Dependecies injection.**
* **SingleTon Design Pattern.**

