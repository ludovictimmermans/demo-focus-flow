FocusFlow – Backend
FocusFlow is the backend service of a productivity application designed to help users organize tasks, track habits, and monitor their progress over time. The project aims to provide a secure, scalable, and maintainable API built with modern Spring Boot practices. This repository currently contains the initial architecture skeleton, prepared before implementing business logic to ensure clarity and long‑term maintainability.
Overview
The backend will expose REST endpoints for authentication, task management, habit tracking, and dashboard aggregation. It is designed with separation of concerns, testability, and enterprise‑grade structure in mind. As development progresses, each module will be implemented following clean architecture principles and strict domain boundaries.
Technology Stack

- Java 21
- Spring Boot 3
- Spring Web
- Spring Data JPA
- Spring Security with JWT
- PostgreSQL
- Flyway for database migrations
- MapStruct for DTO mapping
- OpenAPI/Swagger for API documentation
- Maven for build and dependency management
  Project Structure
  The backend follows a clear and extensible package layout:
  com.focusflow/
  ├── config/ # Application configuration classes
  ├── security/ # JWT handling, authentication filters, security setup
  ├── controller/ # REST controllers exposing API endpoints
  ├── service/ # Business logic and domain rules
  ├── repository/ # Spring Data JPA repositories
  ├── domain/ # Entities, enums, and core domain models
  ├── dto/ # Request and response data transfer objects
  ├── mapper/ # MapStruct mappers for DTO ↔ entity conversion
  ├── exception/ # Global exception handling and error responses
  └── FocusFlowApplication.java

This structure is intentionally created before adding features to ensure a clean foundation and consistent development workflow.
Planned Features

- User registration, login, and profile management
- Secure multi‑user data isolation
- Task CRUD operations with search, filtering, sorting, and pagination
- Habit tracking with check‑ins and streak computation
- Dashboard summarizing tasks and habit progress
- Centralized exception handling with consistent error responses
- Database migrations and seed data using Flyway
  Testing Strategy
- Unit tests for business logic using JUnit 5
- Integration tests with Testcontainers and PostgreSQL
- Continuous integration pipeline using GitHub Actions
  Docker Support
  A docker‑compose setup will be added to orchestrate the backend, frontend, and PostgreSQL database for local development and deployment.
  API Documentation
  Swagger/OpenAPI documentation will be available at /swagger-ui once the API endpoints are implemented.
  Current Status
  The repository currently contains the initial folder structure. Implementation of authentication, domain models, services, and controllers will follow in the next development steps.
