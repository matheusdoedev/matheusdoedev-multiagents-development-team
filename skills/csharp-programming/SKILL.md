Name: C# Programming
Description:

# C# Programming Best Practices

## Description

This skill provides a comprehensive guide to writing high-quality C# code following Microsoft's coding standards, best practices, and effective use of language features. It helps developers produce maintainable, performant, and idiomatic C# applications.

## Scope

- Personal skill for C# developers
- Applicable to .NET Framework, .NET Core, and .NET 5+
- Can be used during coding, code reviews, or refactoring C# projects

## Workflow Steps

### 1. Project Structure and Organization

- Use meaningful namespaces that reflect the project's structure
- Organize code into logical assemblies and folders
- Follow the .NET project layout conventions
- Use consistent file and folder naming

### 2. Naming Conventions

- Use PascalCase for types, methods, and properties
- Use camelCase for parameters, local variables, and private fields
- Use UPPER_CASE for constants
- Prefix interfaces with 'I' (e.g., IService)
- Use descriptive names that convey intent

### 3. Type Design

- Prefer classes over structs unless the type is small, immutable, and logically represents a single value
- Use interfaces to define contracts
- Implement IDisposable for types that hold unmanaged resources
- Use generics to create reusable, type-safe components
- Prefer immutable types when possible

### 4. Method Design

- Keep methods small and focused on a single responsibility
- Use meaningful parameter names and consider optional parameters
- Return IEnumerable<T> instead of List<T> for sequences
- Use async/await for I/O-bound operations
- Handle exceptions appropriately; don't catch general exceptions

### 5. Language Feature Usage

- Use LINQ for querying collections when it improves readability
- Prefer object and collection initializers
- Use null-conditional operators (?.) and null-coalescing operators (??)
- Leverage pattern matching (is, switch expressions)
- Use records for immutable data

### 6. Error Handling and Logging

- Use try-catch blocks judiciously; prefer prevention over handling
- Throw meaningful custom exceptions when appropriate
- Use structured logging with appropriate log levels
- Implement proper resource cleanup with using statements

### 7. Performance Considerations

- Avoid unnecessary allocations in hot paths
- Use StringBuilder for string concatenation in loops
- Consider lazy loading for expensive operations
- Profile and measure performance bottlenecks

### 8. Testing

- Write unit tests for all public APIs
- Use xUnit, NUnit, or MSTest frameworks
- Mock dependencies using Moq or similar libraries
- Follow Arrange-Act-Assert pattern

## Decision Points

- If a method might throw: Use checked exceptions or Result types for functional error handling
- If working with collections: Choose between arrays, List<T>, or more specialized collections
- If needing thread safety: Use Concurrent collections or proper locking mechanisms
- If performance is critical: Profile first, then optimize; avoid premature optimization
- If code is reusable: Extract to a separate library or NuGet package

## Quality Criteria

- Code compiles without warnings (treat warnings as errors)
- Passes all unit tests and integration tests
- Follows Microsoft's C# Coding Conventions
- Achieves good performance metrics
- Receives positive feedback in code reviews
- Is maintainable and extensible

## Common Patterns and Idioms

### Dependency Injection

- Use constructor injection for required dependencies
- Register services in Startup.cs or Program.cs
- Avoid service locator anti-pattern

### Asynchronous Programming

- Use async/await throughout the call stack
- Avoid async void except for event handlers
- Use Task.WhenAll for concurrent operations
- ConfigureAwait(false) in library code

### LINQ Usage

- Use method syntax for complex queries
- Prefer Any(), All(), FirstOrDefault() over Count() > 0
- Chain operations efficiently

### Exception Handling

- Catch specific exceptions, not Exception
- Use finally blocks for cleanup
- Consider using Polly for retry policies

## Example Usage

When implementing a data access layer:

1. Define interfaces for repositories
2. Use Entity Framework Core with async methods
3. Implement proper error handling and logging
4. Write comprehensive unit tests with in-memory database
5. Follow naming conventions and keep methods focused
6. Use dependency injection for testability
