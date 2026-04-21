---
name: solid-practices
description: It is a skill that gives capabilities to apply SOLID principles to achieve maintainable, flexible, and robust object-oriented designs that adapt to changing requirements.
---

- It is a software design style, where the goal is to write code where components are less coupled to each other.

- It is not a good ideia to have a software where the entire application depends of a single component. That makes more difficult to make maintenance, or add more features, because every time I need to make a modification in that component, I must change each component that depend of it.

- Alongside, it is not a good one to have a component that depends of the implementation of another application, instead of depends of the abstract idea (what the component do, instead of how the component do).

- SOLID is a acronym for five principles:
  - S: Single Responsibility Principle;
  - O: Open-Closed Principle;
  - L: Liskov Substitution Principle;
  - I: Interface Segregation Principle;
  - D: Dependency Inversion Principle.

## Single Responsibility Principle

## Scope

- Personal skill for object-oriented developers
- Applicable to all OOP languages
- Can be used for architecture and code review

## Workflow Steps

### 1. Single Responsibility Principle (SRP)

- One reason to change per class
- Clear, focused class purpose
- Avoid god objects
- Separate concerns
- Extract responsibilities to new classes
- Use meaningful class names
- Document responsibility

### 2. Open/Closed Principle (OCP)

- Open for extension
- Closed for modification
- Use inheritance/composition for extension
- Define extension points
- Avoid modifying existing code
- Use interfaces for contracts
- Plan for future changes

### 3. Liskov Substitution Principle (LSP)

- Derived classes are substitutable
- Don't violate type contracts
- Avoid narrowing parameter types
- Avoid widening return types
- Honor pre/post conditions
- Document behavior expectations
- Test substitutability

### 4. Interface Segregation Principle (ISP)

- Small, focused interfaces
- Don't force unnecessary implementations
- Clients depend only on what they use
- Avoid "fat" interfaces
- Create role-based interfaces
- Depend on abstractions
- Document interface contracts

### 5. Dependency Inversion Principle (DIP)

- Depend on abstractions, not implementations
- High-level modules don't depend on low-level
- Use dependency injection
- Invert dependencies
- Program to interfaces
- Use IoC containers
- Avoid tight coupling

### 6. Evaluating SOLID Violations

- Identify tightly coupled code
- Find classes with multiple responsibilities
- Detect rigid class hierarchies
- Recognize fat interfaces
- Spot hardcoded dependencies
- Look for modification patterns
- Document violations

### 7. Refactoring to SOLID

- Extract responsibilities gradually
- Introduce abstractions
- Use design patterns
- Implement dependency injection
- Create interfaces
- Remove duplication
- Improve testability

### 8. Testing SOLID Designs

- Write focused unit tests
- Mock dependencies easily
- Test one responsibility per test
- Avoid test interdependencies
- Verify substitutability
- Test interfaces, not implementations
- Maintain test clarity

## Quality Criteria

- Each class has single responsibility
- Code is open for extension, closed for modification
- Derived classes are substitutable
- Interfaces are focused
- Dependencies flow correctly
- Code is testable
- Code is flexible and maintainable
- Changes require minimal modifications

## Decision Framework

- If class has multiple reasons to change: Apply SRP
- If modification is needed for extension: Apply OCP
- If substitution causes errors: Apply LSP
- If class implements unused methods: Apply ISP
- If dependencies are tightly coupled: Apply DIP

## Common Violations and Fixes

### SRP Violation

**Bad:** User class handling auth, business logic, and data access
**Fix:** Create UserService, AuthService, UserRepository

### OCP Violation

**Bad:** Adding if statements for new types
**Fix:** Use interfaces and polymorphism

### LSP Violation

**Bad:** Override method with incompatible behavior
**Fix:** Honor type contract or redesign hierarchy

### ISP Violation

**Bad:** Interface with many unused methods
**Fix:** Create smaller, focused interfaces

### DIP Violation

**Bad:** Classes creating dependencies directly
**Fix:** Use constructor injection and interfaces

## Example Usage

When refactoring a user management system:

1. Identify SRP violations in large classes
2. Split into focused classes
3. Create interfaces for dependencies
4. Implement dependency injection
5. Remove tight coupling
6. Apply design patterns
7. Verify with unit tests
