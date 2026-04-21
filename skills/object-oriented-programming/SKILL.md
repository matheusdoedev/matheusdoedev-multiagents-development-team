---
name: object-oriented-programming
description: Workflow for writing well-designed object-oriented code, emphasizing encapsulation, inheritance, polymorphism, and proper use of OOP principles.
keywords: OOP, objects, classes, inheritance, polymorphism, encapsulation, design
---

## Description

This skill provides a workflow for writing effective object-oriented code. It emphasizes the four pillars of OOP: encapsulation, inheritance, polymorphism, and abstraction.

## Scope

- Personal skill for all developers using OOP languages
- Applicable to Java, C#, Python, and other OOP languages
- Can be used for class design and code organization

## Workflow Steps

### 1. Encapsulation

- Hide internal state
- Use access modifiers (private, public, protected)
- Provide getter/setter methods when appropriate
- Avoid exposing internal data structures
- Maintain class invariants
- Validate input in setters
- Document public interface

### 2. Classes and Objects

- Design classes with single responsibility
- Use meaningful class names
- Define clear interfaces
- Implement constructors properly
- Initialize state correctly
- Provide appropriate methods
- Document class purpose

### 3. Inheritance

- Use inheritance for "is-a" relationships
- Avoid deep inheritance hierarchies
- Call super constructor
- Override methods intentionally
- Use abstract base classes
- Implement interface contracts
- Document inheritance purpose

### 4. Polymorphism

- Use method overriding
- Implement interface polymorphism
- Use method overloading appropriately
- Design for liskov substitution principle
- Avoid type checking in loops
- Use polymorphic collections
- Leverage dynamic dispatch

### 5. Abstraction

- Create abstract classes for shared behavior
- Define interfaces for contracts
- Hide implementation details
- Expose behavior, not state
- Use meaningful abstractions
- Avoid leaky abstractions
- Document abstraction level

### 6. Composition vs Inheritance

- Prefer composition over inheritance
- Use inheritance for true hierarchies
- Design flexible compositions
- Avoid fragile base class problem
- Implement delegation patterns
- Use mixins/traits when available
- Document design choice

### 7. Design Patterns

- Apply Gang of Four patterns
- Use creational patterns (Factory, Builder)
- Use structural patterns (Adapter, Decorator)
- Use behavioral patterns (Observer, Strategy)
- Document pattern usage
- Avoid over-engineering
- Balance simplicity with flexibility

### 8. Code Organization

- Organize classes logically
- Use packages/namespaces
- Manage dependencies
- Maintain clear module structure
- Avoid circular dependencies
- Document module relationships
- Plan for extensibility

## Quality Criteria

- Classes have clear responsibilities
- Encapsulation is maintained
- Inheritance is used appropriately
- Polymorphism is leveraged effectively
- Code is extensible
- Dependencies are manageable
- Abstractions are clear
- Design follows SOLID principles

## Decision Points

- If relationship is "is-a": Use inheritance
- If relationship is "has-a": Use composition
- If multiple implementations: Use interfaces
- If behavior varies by type: Use polymorphism
- If logic is complex: Extract into separate classes
- If code is repetitive: Use abstraction

## Example Usage

When designing a payment system:

1. Create abstract PaymentMethod class
2. Implement CreditCard, PayPal, etc. as subclasses
3. Use polymorphism for payment processing
4. Encapsulate payment logic
5. Use composition for address/account info
6. Implement appropriate interfaces
7. Organize into logical packages
