Todolist Application
The Todolist application is a simple REST API built with Spring Boot, designed for managing tasks in a to-do list. It uses Spring Data JPA for database interactions, MySQL for data storage, and Lombok to reduce boilerplate code. This project demonstrates a clean architecture with layers for controllers, services, and repositories.

To set up the project, ensure you have Java 11 or higher, Gradle, and a running MySQL database. First, create a database named todolist. Then, configure the database connection in src/main/resources/application.properties by specifying the spring.datasource.url, spring.datasource.username, and spring.datasource.password. Use gradlew bootRun to start the application, which will be accessible at http://localhost:8080.

The API provides endpoints for creating, retrieving, updating, and deleting tasks. You can use tools like Postman or cURL to interact with the API. Example endpoints include /api/tasks to fetch all tasks, and /api/tasks/{id} to fetch, update, or delete a specific task. Tasks have fields for title, description, and completed status.

Dependencies like spring-boot-starter-web and spring-boot-starter-data-jpa power the web layer and database interactions, while mysql-connector-java ensures connectivity to the database. Run gradlew build to resolve dependencies and compile the project. Use gradlew clean build for a clean rebuild if needed.

This project is an excellent starting point for learning Spring Boot and building REST APIs with robust database support. It can be extended further by adding features like authentication, advanced validations, and exception handling.