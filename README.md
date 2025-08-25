# Spring Boot User API

A lightweight RESTful API built with Spring Boot, H2 Database, and Spring Data JPA. Supports full CRUD operations for managing users.

## 🚀 Features

- REST endpoints for user management (`GET`, `POST`, `PUT`, `DELETE`)
- In-memory H2 database with auto schema generation
- Spring Data JPA for easy persistence
- Maven-based build and run
- Ready for containerization and CI/CD integration

## 📦 Tech Stack

- Java 17+
- Spring Boot
- Spring Web
- Spring Data JPA
- H2 Database
- Maven

## 📁 Project Structure
src/ ├── main/ │ ├── java/com/example/user/ │ │ ├── controller/ # REST controllers │ │ ├── model/ # JPA entities │ │ ├── repository/ # Spring Data JPA interfaces │ │ ├── service/ # Business logic │ │ └── UserApplication.java │ └── resources/ │ ├── application.properties │ └── data.sql # Optional: preload sample users

Code

## 🧪 API Endpoints

| Method | Endpoint           | Description         |
|--------|--------------------|---------------------|
| GET    | `/api/users`       | Get all users       |
| GET    | `/api/users/{id}`  | Get user by ID      |
| POST   | `/api/users`       | Create new user     |
| PUT    | `/api/users/{id}`  | Update user         |
| DELETE | `/api/users/{id}`  | Delete user         |

## 🛠️ Running Locally

```bash
./mvnw spring-boot:run
Then visit:

http://localhost:8080/api/users

http://localhost:8080/h2-console (JDBC URL: jdbc:h2:mem:testdb)

