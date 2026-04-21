---
name: angular
description: Workflow for building robust, scalable single-page applications using Angular framework, emphasizing dependency injection, components, services, and TypeScript patterns.
keywords: Angular, TypeScript, SPA, components, services, dependency injection
---

## Description

This skill provides a workflow for building enterprise-grade SPAs using Angular. It emphasizes proper component architecture, service design, dependency injection, reactive programming, and scalability.

## Scope

- Personal skill for frontend developers using Angular
- Applicable to Angular 14+
- Can be used for component development, service design, and application architecture

## Workflow Steps

### 1. Angular Project Setup

- Create project with Angular CLI
- Understand project structure and conventions
- Configure TypeScript for Angular
- Set up development environment
- Understand angular.json configuration
- Use lazy loading for modules

### 2. Component Architecture

- Create components for specific features
- Use component selectors appropriately
- Implement input/output properties
- Use lifecycle hooks correctly
- Implement OnInit for initialization
- Clean up resources in OnDestroy

### 3. Services and Dependency Injection

- Create services for business logic
- Use dependency injection for services
- Implement singleton patterns with services
- Create provider configuration
- Use factory providers when needed
- Understand service scopes

### 4. Data Binding and Templates

- Use interpolation correctly
- Implement property and event binding
- Use two-way binding appropriately
- Use structural directives (*ngIf, *ngFor)
- Create attribute directives
- Use safe navigation operator

### 5. Reactive Programming with RxJS

- Use Observables for data streams
- Use operators (map, filter, switchMap)
- Implement async pipe for subscriptions
- Handle Subjects and BehaviorSubjects
- Unsubscribe properly to avoid memory leaks
- Compose complex data flows

### 6. Routing

- Configure routes with RouterModule
- Implement lazy loading for modules
- Use route guards for protection
- Handle route parameters
- Implement nested routing
- Use routing best practices

### 7. Forms

- Use Reactive Forms for complex forms
- Use FormBuilder for form creation
- Implement validation rules
- Handle form submission
- Implement error display
- Test form logic

### 8. Testing

- Write unit tests with Jasmine
- Use TestBed for component testing
- Mock services appropriately
- Test component interaction
- Achieve adequate coverage
- Test async operations

## Quality Criteria

- Components follow Angular conventions
- Services are well-designed and testable
- Dependency injection is used properly
- Reactive patterns are implemented correctly
- Templates are clean and readable
- Routing is well-organized
- Tests cover business logic
- Application is performant

## Example Usage

When building a user management feature:

1. Create components for list and detail views
2. Implement UserService for API communication
3. Use Observables for data streams
4. Configure routing with lazy loading
5. Implement guards for protected routes
6. Create forms with validation
7. Write comprehensive tests
