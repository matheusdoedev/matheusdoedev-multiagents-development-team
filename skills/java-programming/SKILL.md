---
name: java-programming
description: Comprehensive workflow for writing clean, efficient Java code following modern best practices, emphasizing type safety, concurrency, performance optimization, and enterprise patterns.
keywords: Java, OOP, concurrency, performance, Spring, design patterns, JVM
---

## Description

This skill provides a workflow for writing high-quality Java code. It emphasizes modern Java features, performance optimization, proper exception handling, concurrency patterns, and adherence to Java best practices.

## Scope

- Personal skill for Java developers
- Applicable to Java 11+ projects
- Can be used for backend development, system design, and code reviews

## Workflow Steps

### 1. Java Language Features

- Use modern Java features (var, records, sealed classes)
- Leverage functional programming with streams
- Use optionals instead of null checks
- Implement lambda expressions effectively
- Use proper generics and type parameters
- Understand type erasure and raw types
- Use enhanced for loops appropriately

### 2. Object-Oriented Design

- Design classes with single responsibility
- Use inheritance judiciously
- Prefer composition over inheritance
- Implement interfaces for contracts
- Use abstract classes appropriately
- Encapsulate data properly
- Document public contracts

### 3. Exception Handling

- Use checked exceptions for recoverable errors
- Use runtime exceptions for programming errors
- Never catch generic Exception
- Provide meaningful exception messages
- Clean up resources with try-with-resources
- Implement proper error logging
- Document thrown exceptions

### 4. Collections and Streams

- Choose appropriate collection types
- Use Collections framework properly
- Leverage streams for data processing
- Understand stream laziness
- Use terminal operations correctly
- Avoid collecting everything into lists
- Consider performance implications

### 5. Concurrency

- Use synchronized appropriately
- Understand volatile keyword
- Use concurrent collections
- Implement proper locking
- Avoid deadlocks
- Use ExecutorService for thread pools
- Handle InterruptedException properly

### 6. Performance Optimization

- Profile before optimizing
- Understand JVM garbage collection
- Minimize object allocations
- Use StringBuilder for string concatenation
- Implement caching strategically
- Monitor memory usage
- Profile hotspots

### 7. Testing

- Write unit tests with JUnit
- Use mocking frameworks (Mockito)
- Test exception scenarios
- Implement integration tests
- Achieve adequate coverage
- Use parameterized tests
- Keep tests maintainable

### 8. Package Structure and Dependencies

- Organize packages by feature
- Avoid circular dependencies
- Use appropriate visibility modifiers
- Manage transitive dependencies
- Keep dependencies minimal
- Use dependency injection
- Document module structure

## Decision Points

- If method is large: Break into smaller methods with clear names
- If complexity is high: Extract into separate classes or methods
- If null handling is complex: Use Optional effectively
- If performance is critical: Profile first, then optimize
- If threading is involved: Use concurrent utilities from java.util.concurrent
- If object creation is expensive: Consider object pooling or caching

## Quality Criteria

- Code compiles without warnings
- All tests pass
- Code follows Java conventions
- Performance is acceptable
- Concurrency is handled correctly
- Exceptions are handled properly
- Code is maintainable and readable
- Dependencies are managed well

## Common Patterns and Best Practices

### Null Safety

```java
Optional<String> value = getValue();
String result = value.orElse("default");
```

### Streams

```java
list.stream()
    .filter(x -> x > 10)
    .map(x -> x * 2)
    .collect(Collectors.toList());
```

### Try-With-Resources

```java
try (FileInputStream fis = new FileInputStream(file)) {
    // Use resource
} catch (IOException e) {
    // Handle error
}
```

## Example Usage

When implementing a data processing service:

1. Design classes with single responsibility
2. Use Optional for nullable returns
3. Implement streams for data processing
4. Add proper exception handling
5. Use concurrent collections if multi-threaded
6. Write comprehensive unit tests
7. Monitor performance with profiling
