JWT - post API:-
Username: admin
Password: admin123

Swagger URL: http://localhost:8088/swagger-ui/index.html#/

# File-Processing-with-JWT-Authentication
This project is a Spring Boot-based microservice designed to manage Skills, Jobs, and Tasks data. It provides RESTful APIs for CRUD operations and bulk updates of job/task-related data. The project includes JWT-based authentication and Swagger integration for API documentation and testing

Key Features:-
Skill, Job, and Task Management
CRUD operations for skills.
Fetch, update, and delete job/task information.
Maintain relationships between jobs, tasks, and skill uploads.

Security:-
JWT Authentication secures all endpoints except /auth/login and Swagger endpoints.
AuthController provides /auth/login endpoint to generate JWT tokens for authenticated users.
JwtRequestFilter intercepts requests to validate JWT and populate Spring Security context.

API Documentation:-
Integrated Swagger UI for interactive API documentation.
Provides endpoint testing and JWT authentication via Swagger’s “Authorize” feature.

Utilities:-
ReaderUtil handles Excel file reading for jobs, tasks, and skill uploads.
Common parsing, validation, and logging methods are centralized for reuse.

Technology Stack:-
Spring Boot (REST APIs, Security, Dependency Injection)
Spring Security + JWT (Authentication & Authorization)
Swagger/OpenAPI (API documentation)
Apache POI (Excel file processing)
Maven (Project management)
PostgreSQL
