---
name: nodejs
description: Workflow for building scalable, maintainable backend applications using Node.js, emphasizing server architecture, async patterns, REST APIs, error handling, and deployment best practices.
keywords: Node.js, backend, Express, async, APIs, performance, scalability
---

## Description

This skill provides a comprehensive workflow for building robust backend applications with Node.js. It emphasizes clean architecture, async/await patterns, RESTful API design, error handling, and deployment practices.

## Scope

- Personal skill for backend developers using Node.js
- Applicable to Express, Fastify, and other Node.js frameworks
- Can be used for API development, server configuration, and optimization

## Workflow Steps

### 1. Project Structure and Organization

- Organize code into meaningful layers: routes, controllers, services, models
- Use middleware appropriately for cross-cutting concerns
- Separate concerns into different modules
- Use consistent folder structure across projects
- Keep configuration separate from business logic

### 2. Asynchronous Programming

- Use async/await consistently throughout the application
- Avoid callback hell; prefer Promises or async/await
- Handle all async errors properly
- Use Promise.all() for concurrent operations
- Implement proper error handling in async functions
- Be aware of blocking operations

### 3. REST API Design

- Follow REST principles for API design
- Use appropriate HTTP methods (GET, POST, PUT, DELETE)
- Return meaningful status codes
- Provide consistent error responses
- Implement pagination for large datasets
- Use proper request validation

### 4. Middleware and Request Handling

- Use middleware to handle cross-cutting concerns
- Order middleware appropriately
- Validate user input before processing
- Implement authentication and authorization
- Add request logging
- Use error-handling middleware

### 5. Data Persistence

- Use appropriate database drivers or ORMs
- Implement database connection pooling
- Use transactions for data consistency
- Optimize database queries
- Handle database errors gracefully
- Implement proper schema design

### 6. Error Handling

- Create custom error classes
- Implement global error handler middleware
- Log errors appropriately
- Provide meaningful error messages to clients
- Handle validation errors properly
- Distinguish between client and server errors

### 7. Security

- Validate all user input
- Use parameterized queries to prevent SQL injection
- Implement rate limiting
- Use HTTPS for production
- Implement CORS properly
- Securely manage environment variables
- Use authentication tokens (JWT) correctly

### 8. Performance and Scalability

- Use caching strategies (Redis)
- Implement load balancing
- Optimize database queries
- Use compression for responses
- Monitor and profile applications
- Use clustering for multi-core systems

### 9. Testing

- Write unit tests for business logic
- Write integration tests for API endpoints
- Mock external dependencies
- Achieve adequate test coverage
- Use appropriate testing frameworks

### 10. Deployment

- Use environment variables for configuration
- Implement proper logging
- Use process managers (PM2)
- Set up monitoring and alerting
- Implement graceful shutdown
- Document deployment process

## Quality Criteria

- Code is well-organized and modular
- All endpoints are properly documented
- Error handling is comprehensive
- Security best practices are followed
- Performance meets requirements
- All tests pass
- Code follows linting rules
- Deployment process is automated

## Example Usage

When building a user API:

1. Structure with routes, controllers, services
2. Implement CRUD endpoints with validation
3. Add middleware for authentication
4. Use async/await for data operations
5. Implement comprehensive error handling
6. Write integration tests
7. Add logging and monitoring
8. Deploy with environment configuration
