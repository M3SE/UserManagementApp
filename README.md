## Mini Spring Boot Project: User Management App
## Objective: 
- Create a Spring Boot application that implements user management functionalities, integrating validation, security, database connectivity, and exception handling.


## Description of Each Package:
1. com.example.demo (Root Package):
- UserManagementAppApplication.java: This is the main entry point of your Spring Boot application, containing the @SpringBootApplication annotation.
2. config:
- Purpose: Contains configuration classes, such as those for Spring Security, CORS configuration, or any other application-wide configuration.
- Example: SecurityConfig.java for configuring Spring Security, custom authentication, etc.
3. controller:
- Purpose: Contains your REST controllers, which handle HTTP requests and map them to service layer calls.
- Example: UserController.java for managing user-related endpoints like registration, login, etc.
4. dto (Data Transfer Objects):
- Purpose: Contains DTOs used to transfer data between layers, especially for request and response bodies.
- Example: UserRegistrationDto.java to encapsulate data for user registration.
5. exception:
- Purpose: Contains custom exceptions and global exception handling mechanisms.
- Example: GlobalExceptionHandler.java to manage application-wide error handling, ensuring consistent responses.
6. model:
- Purpose: Contains your JPA entities that map to database tables.
- Example: User.java representing the User entity with fields like id, username, password, and email.
7. repository:
- Purpose: Contains Spring Data JPA repository interfaces for data access.
- Example: UserRepository.java for performing CRUD operations on the User entity.
8. service:
- Purpose: Contains service classes that encapsulate business logic.
- Example: UserService.java for handling operations related to users, such as saving new users, fetching user details, etc.
9. util (Optional):
- Purpose: Contains utility classes that provide shared methods or functionalities that can be reused across the application.
- Example: ValidationUtils.java for custom validation logic that might be used across multiple DTOs or entities.