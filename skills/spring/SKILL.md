---
name: spring
description: Workflow for building scalable enterprise applications using Spring Framework, emphasizing dependency injection, configuration, REST APIs, security, and production patterns.
keywords: Spring, Spring Boot, dependency injection, REST APIs, security, transactions
---

## Description

This skill provides a workflow for building robust enterprise applications using Spring Framework. It emphasizes proper component design, configuration management, REST API development, and security implementation.

## Scope

- Personal skill for Java backend developers
- Applicable to Spring Framework 5.x and Spring Boot 2.x+
- Can be used for API development, service architecture, and deployment

## Workflow Steps

### 1. Spring Boot Project Setup

- Create project with Spring Boot
- Configure application.yml or application.properties
- Understand auto-configuration
- Configure server settings
- Set up profiles for environments
- Configure logging
- Manage dependencies with Maven/Gradle

### 2. Dependency Injection

- Use @Component, @Service, @Repository, @Controller
- Implement constructor injection
- Configure beans appropriately
- Use @Autowired judiciously (prefer constructor)
- Implement custom beans with @Bean
- Manage bean scopes
- Configure component scanning

### 3. REST API Development

- Create REST endpoints with @RestController
- Use @RequestMapping, @GetMapping, @PostMapping
- Implement proper HTTP methods
- Validate input with @Valid
- Implement error handling
- Use ResponseEntity for responses
- Document with Swagger/OpenAPI

### 4. Service Layer

- Implement business logic in @Service classes
- Use @Transactional appropriately
- Implement proper error handling
- Manage dependencies properly
- Implement caching with @Cacheable
- Use @Async for async operations
- Keep services testable

### 5. Data Access

- Use Spring Data repositories
- Implement custom queries
- Use JPA/Hibernate effectively
- Configure database connections
- Implement transaction management
- Handle entity relationships
- Optimize database access

### 6. Security

- Implement authentication with Spring Security
- Configure authorization rules
- Use JWT tokens when appropriate
- Secure sensitive endpoints
- Implement rate limiting
- Configure HTTPS
- Handle credentials securely

### 7. Configuration and Profiles

- Use externalized configuration
- Implement environment-specific configs
- Use @ConfigurationProperties
- Set up development/test/production profiles
- Manage secrets appropriately
- Document configuration options
- Test configuration

### 8. Testing

- Write unit tests with JUnit and Mockito
- Write integration tests with @SpringBootTest
- Mock services appropriately
- Test REST endpoints
- Test database interactions
- Achieve adequate coverage
- Keep tests maintainable

## Quality Criteria

- Application follows Spring conventions
- Components are loosely coupled
- Configuration is externalized
- REST APIs are well-designed
- Security is properly implemented
- Error handling is comprehensive
- Tests cover business logic
- Performance is optimized

## Common Patterns

### REST Endpoint

```java
@RestController
@RequestMapping("/api/users")
public class UserController {
    @PostMapping
    public ResponseEntity<UserDTO> create(@Valid @RequestBody CreateUserRequest req) {
        UserDTO user = userService.create(req);
        return ResponseEntity.status(HttpStatus.CREATED).body(user);
    }
}
```

### Service with Transactions

```java
@Service
@Transactional
public class UserService {
    public void updateUser(UserDTO dto) {
        User user = userRepository.findById(dto.getId()).orElseThrow();
        user.update(dto);
        userRepository.save(user);
    }
}
```

## Example Usage

When building a user management API:

1. Create Spring Boot project
2. Configure database connection
3. Define JPA entities
4. Create Spring Data repositories
5. Implement service layer
6. Create REST endpoints
7. Add Spring Security
8. Write comprehensive tests
