FocusFlow – Backend
FocusFlow is the backend service of a productivity application designed to help users manage tasks, track habits, and monitor their progress. This module provides a structured Spring Boot foundation prepared for secure, scalable feature development.
Project Overview
The backend exposes a REST API that will support authentication, task management, habit tracking, and dashboard data aggregation. The current state of the repository contains the initial architecture skeleton, created before implementing business logic to ensure clarity and maintainability.
Technology Stack
• Java 21
• Spring Boot 3
• Spring Web
• Spring Data JPA
• Spring Security with JWT
• PostgreSQL
• Flyway
• MapStruct
• OpenAPI/Swagger
• Maven
Project Structure
The backend follows a clean, domain‑oriented package layout:
com.focusflow/
├── config/ # Application configuration
├── security/ # Authentication and JWT handling
├── controller/ # REST controllers
├── service/ # Business logic
├── repository/ # JPA repositories
├── domain/ # Entities and enums
├── dto/ # Request and response models
├── mapper/ # MapStruct mappers
├── exception/ # Global exception handling
└── FocusFlowApplication.java

This structure is intentionally created before adding features to ensure a clear separation of concerns and a scalable architecture.
Planned Features

- User registration, login, and profile management
- Secure multi‑user data isolation
- Task CRUD operations with filtering, search, and pagination
- Habit tracking with streak computation
- Dashboard summarizing user activity
- Comprehensive error handling and validation
  Testing Strategy
- Unit tests for business rules using JUnit 5
- Integration tests using Testcontainers with PostgreSQL
- Continuous integration through GitHub Actions
  Docker
  A docker-compose setup will orchestrate the backend, frontend, and PostgreSQL database once the implementation is complete.
  API Documentation
  Swagger/OpenAPI documentation will be available at /swagger-ui after the API endpoints are implemented.
  Status
  The backend currently contains the initial folder structure. Implementation of authentication, domain models, services, and controllers will follow.
