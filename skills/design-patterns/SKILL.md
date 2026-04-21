# Design Patterns Implementation

## Description

This skill provides a structured workflow for identifying software design problems, selecting appropriate design patterns, and implementing them correctly. It helps developers apply Gang of Four patterns and other common patterns to improve code structure, reusability, and maintainability.

## Scope

- Personal skill for software developers
- Primarily applicable to object-oriented programming languages (Java, C#, Python, etc.)
- Can be used during design phases, refactoring, or when encountering recurring problems

## Workflow Steps

### 1. Problem Analysis

- Identify the core problem or requirement
- Determine the type of problem: creation, structural, or behavioral
- Assess constraints: performance, complexity, extensibility needs
- Look for recurring patterns in the codebase

### 2. Pattern Selection

- Review common patterns for the problem type:
  - Creational: Singleton, Factory, Builder, Prototype
  - Structural: Adapter, Decorator, Facade, Composite, Proxy
  - Behavioral: Observer, Strategy, Command, Iterator, State, Template Method
- Evaluate pattern fit based on:
  - Complexity vs. benefit
  - Language/framework support
  - Team familiarity

### 3. Implementation Planning

- Sketch the class diagram or structure
- Identify participants (classes/interfaces involved)
- Plan the integration with existing code
- Consider testing approach

### 4. Code Implementation

- Create the necessary classes and interfaces
- Implement the pattern structure
- Ensure proper encapsulation and abstraction
- Add comments explaining the pattern usage

### 5. Integration and Testing

- Integrate the pattern into the existing codebase
- Write unit tests for the pattern implementation
- Test edge cases and interactions
- Refactor if needed to fit the overall architecture

### 6. Documentation and Review

- Document the pattern usage and benefits
- Review with team members for feedback
- Update any relevant design documents

## Decision Points

- If the problem is about object creation: Choose creational patterns
- If the problem involves class composition: Consider structural patterns
- If the problem is about object interaction: Use behavioral patterns
- If a pattern increases complexity without clear benefits: Consider simpler solutions
- If the team is unfamiliar with a pattern: Provide training or choose alternatives

## Quality Criteria

- The pattern solves the identified problem effectively
- Code remains readable and maintainable
- Implementation follows the standard pattern structure
- Unit tests cover the pattern's behavior
- The solution is extensible for future changes
- Performance requirements are met

## Common Patterns and Use Cases

### Creational Patterns

- **Singleton**: Ensure single instance (e.g., configuration manager)
- **Factory**: Create objects without specifying exact classes
- **Builder**: Construct complex objects step-by-step
- **Prototype**: Clone existing objects

### Structural Patterns

- **Adapter**: Convert interface to another expected interface
- **Decorator**: Add behavior dynamically
- **Facade**: Provide unified interface to subsystem
- **Composite**: Treat individual and composite objects uniformly

### Behavioral Patterns

- **Observer**: Notify dependents of state changes
- **Strategy**: Encapsulate algorithms
- **Command**: Encapsulate requests as objects
- **Iterator**: Access elements sequentially
- **State**: Change behavior based on state
- **Template Method**: Define algorithm skeleton

## Example Usage

When designing a notification system:

1. Analyze: Need to notify multiple subscribers of events
2. Select: Observer pattern fits perfectly
3. Plan: Subject interface, ConcreteSubject, Observer interface, ConcreteObservers
4. Implement: Create the classes with proper relationships
5. Test: Verify notifications are sent correctly
6. Document: Explain why Observer was chosen and how it works
