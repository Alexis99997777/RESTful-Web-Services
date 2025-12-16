RESTful Web Services with Spring Boot

This project is a RESTful Web Service built with Spring Boot, created as part of learning and practicing core backend concepts such as request mapping, dependency injection, validation, exception handling, and standalone deployment.

The application demonstrates how to build a clean REST API using Spring Boot, following best practices such as layered architecture and constructor-based dependency injection.

🚀 Features Implemented

This project includes the following key Spring Boot and RESTful API features:

✅ Project Setup

Create a Spring Boot project using Spring Boot Initializr

Run the web service as a standalone application (embedded Tomcat)

✅ REST Controller & Request Mapping

@RestController and @RequestMapping

Handle HTTP methods:

GET

POST

PUT

DELETE

✅ Request Data Handling

Read Path Variables using @PathVariable

Read Query Parameters using @RequestParam

Required and optional parameters

Read HTTP POST request body using @RequestBody

✅ Validation

Validate request body using @Valid

Bean validation annotations (e.g. @NotNull, @Size, etc.)

✅ Response Handling

Return Java objects as HTTP responses

Automatic conversion to JSON / XML

Set HTTP response status codes using:

ResponseEntity

@ResponseStatus

✅ Temporary Data Storage

Store users temporarily using an in-memory data structure (e.g. Map)

✅ Exception Handling

Global exception handling

Custom error message objects

Handle:

Generic exceptions

Specific exceptions

Custom-defined exceptions

Catch multiple exceptions with a single handler method

✅ Dependency Injection

Create a Service Layer

Use @Service annotation

Constructor-based Dependency Injection

@Autowired dependency resolution by Spring IoC container

🏗 Project Architecture

The project follows a layered architecture:

Controller Layer
    ↓
Service Layer
    ↓
Utility / Data Layer (temporary storage)


Controller Layer
Handles HTTP requests and responses.

Service Layer
Contains business logic.

Utility Classes
Shared helper logic (e.g. ID generation).

🧠 Key Concepts Practiced

RESTful API design

Spring IoC Container & Spring Beans

Dependency Injection (Field vs Constructor-based)

Request lifecycle vs Bean lifecycle

Standalone Spring Boot application execution

Separation of concerns

▶️ Running the Application
Option 1: Run from IDE

Run the main Spring Boot application class directly from your IDE (Eclipse / IntelliJ).

Option 2: Run as Standalone Application

Build the project:

mvn clean package


Run the generated JAR:

java -jar target/your-application-name.jar


The application will start on:

http://localhost:8080

🧪 Testing the API

You can test the API using:

Postman

curl

Browser (for GET requests)

Example:

GET http://localhost:8080/users/{userId}

📦 Technologies Used

Java

Spring Boot

Spring Web

Maven

Embedded Tomcat

JSON / XML serialization

📚 Learning Purpose

This project was created for learning and practicing Spring Boot RESTful web services, focusing on understanding:

How Spring handles HTTP requests

How dependency injection works internally

How to structure a backend application properly
