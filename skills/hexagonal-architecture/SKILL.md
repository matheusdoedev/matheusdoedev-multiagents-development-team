# Hexagonal Architecture Implementation

## Description

This skill provides a comprehensive workflow for designing and implementing applications using Hexagonal Architecture (also known as Ports and Adapters). It helps separate business logic from external concerns, making systems more testable, maintainable, and adaptable to change.

## Scope

- Personal skill for software architects and developers
- Applicable to any programming language and framework
- Can be used for new applications or refactoring existing ones

## Workflow Steps

### 1. Domain Analysis

- Identify core business entities and domain objects
- Define business rules and invariants
- Determine the application's use cases and workflows
- Establish the bounded contexts if using Domain-Driven Design

### 2. Define Ports

- Identify driving ports (interfaces for commands/queries from external actors)
- Identify driven ports (interfaces for external services the application depends on)
- Define port interfaces with clear contracts
- Ensure ports are technology-agnostic

### 3. Implement Adapters

- Create primary adapters (controllers, CLI, API endpoints) that implement driving ports
- Create secondary adapters (repositories, external API clients) that implement driven ports
- Implement dependency injection to connect adapters to the core
- Handle data transformation between external formats and domain objects

### 4. Structure the Application Layers

- Organize code into layers: Domain (core), Application (use cases), Infrastructure (adapters)
- Ensure dependencies point inward (infrastructure depends on application, application on domain)
- Implement application services that orchestrate domain objects
- Keep the domain layer free of external dependencies

### 5. Testing Strategy

- Write unit tests for domain logic without external dependencies
- Test adapters in isolation using mocks/stubs
- Implement integration tests for adapter interactions
- Use test doubles for external services

### 6. Configuration and Deployment

- Configure adapter implementations based on environment
- Implement health checks and monitoring
- Set up deployment pipelines that can swap adapters
- Document adapter configurations and dependencies

## Decision Points

- If an external system changes frequently: Use an adapter to isolate the change
- If business logic needs to be framework-independent: Keep it in the domain layer
- If multiple delivery mechanisms are needed: Implement multiple primary adapters
- If external service is unreliable: Add circuit breakers or retries in the adapter
- If domain logic is complex: Consider splitting into multiple bounded contexts

## Quality Criteria

- Business logic is fully testable without external dependencies
- External changes don't affect core domain code
- Multiple UI frameworks or data stores can be plugged in easily
- Application can be run and tested without infrastructure setup
- Code follows the dependency inversion principle
- Ports define clear, stable interfaces

## Key Concepts

### Ports

- **Driving Ports**: Interfaces that define how external actors (users, systems) interact with the application
- **Driven Ports**: Interfaces that define how the application interacts with external services

### Adapters

- **Primary Adapters**: Controllers, presenters, CLI tools that translate external inputs to domain commands
- **Secondary Adapters**: Repositories, external API clients that translate domain requests to external calls

### Application Structure

```
├── domain/
│   ├── entities/
│   ├── services/
│   └── ports/
├── application/
│   └── use_cases/
└── infrastructure/
    ├── primary_adapters/
    └── secondary_adapters/
```

## Example Usage

When building a user registration system:

1. Domain: Define User entity with validation rules
2. Ports: IUserRepository interface, IEmailService interface
3. Adapters: Implement repository with database, email service with SMTP
4. Application: Create RegisterUser use case that orchestrates validation and persistence
5. Test: Unit test the use case with mock adapters
6. Deploy: Configure different adapters for different environments
