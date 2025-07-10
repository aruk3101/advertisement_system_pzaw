# Back-End of the Advertisement System – Unfinished School Project

## Description

This is the back-end part of an unfinished school project. The project follows a **facade-based structure**, separating responsibilities into clearly organized layers.

Key features include:
- `Dockerfile` for temporary deployment on [Render](https://render.com/)
- Liquibase database migrations
- Checkstyle configuration for code quality
- Environment-specific `application.properties` via environment variables
- JWT token-based authentication
- Resource handling
- API documentation with Swagger

## Structure

### Facades

In most cases, the structure of a facade follows this pattern:

- **Facade Directory**
  - `domain/`
    - `command/`
      - Entity class
      - Entity mapper
      - Entity repository
      - CRUD use cases
      - Validation helpers
      - Facade class
      - Facade configuration
    - `dto/`
      - CRUD DTOs
    - `enumerated/`
      - Optional enumerated values
    - `exception/`
      - Custom exceptions related to the facade
  - Controller class (e.g. `UserController`)

### `resources/` directory

Contains Liquibase changelogs and environment-specific application configuration (`application-local.properties`).

### `upload/` directory

Stores files uploaded by users.

## How to Launch

This app was developed using IntelliJ IDEA Community Edition. To run it, use a custom **Maven Run/Debug configuration** with:

- Command: `spring-boot:run`
- Environment variable: `spring.profiles.active=local` adjusted to the launching environment(local/deploy)

Predefined user with super admin role:
- login : `draczeprojekt@gmail.com` 
- password: `1234`