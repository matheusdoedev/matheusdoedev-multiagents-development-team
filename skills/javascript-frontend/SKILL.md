---
name: javascript-frontend
description: Workflow for writing clean, maintainable, and performant frontend JavaScript following modern ES6+ standards, design patterns, and best practices for interactive web applications.
keywords: JavaScript, frontend, ES6, async, DOM manipulation, events, performance
---

## Description

This skill provides a comprehensive workflow for writing high-quality frontend JavaScript. It focuses on modern ES6+ syntax, asynchronous programming, DOM manipulation, performance optimization, and best practices for building interactive user interfaces.

## Scope

- Personal skill for frontend developers
- Applicable to vanilla JavaScript and framework-independent patterns
- Can be used for component development, performance optimization, and code reviews

## Workflow Steps

### 1. ES6+ Features and Modern Syntax

- Use const/let instead of var for better scoping
- Use arrow functions for concise syntax and lexical this binding
- Leverage destructuring for objects and arrays
- Use template literals for string interpolation
- Use spread operator for arrays and objects
- Use optional chaining (?.) and nullish coalescing (??)
- Prefer for...of loops and functional methods (map, filter, reduce)

### 2. Asynchronous Programming

- Use async/await for cleaner asynchronous code
- Use Promises for async operations
- Handle errors with try/catch in async functions
- Avoid callback hell; use Promise chains or async/await
- Use Promise.all() for concurrent operations
- Handle promise rejections appropriately

### 3. DOM Manipulation

- Query the DOM efficiently using querySelector
- Avoid unnecessary DOM updates in loops
- Use event delegation for dynamic content
- Use addEventListener for event handling, remove with removeEventListener
- Cache DOM references to avoid repeated queries
- Use textContent instead of innerHTML when safe

### 4. Functions and Scope

- Keep functions small and focused on single responsibility
- Use pure functions when possible
- Understand closure and scope properly
- Use function parameters instead of global variables
- Document function parameters and return types
- Use default parameters and rest parameters

### 5. Object-Oriented Programming

- Use classes for object creation with clear structure
- Implement methods appropriately
- Use getters/setters for property access
- Avoid mutating objects; prefer immutability
- Use inheritance carefully; prefer composition
- Implement proper encapsulation

### 6. Performance Optimization

- Use requestAnimationFrame for animations
- Debounce and throttle event handlers
- Lazy load resources
- Minimize DOM reflows and repaints
- Use event delegation
- Optimize loops and calculations
- Use Web Workers for heavy computations

### 7. Module System

- Use ES6 import/export for module organization
- Organize code into logical modules
- Keep module dependencies manageable
- Avoid circular dependencies
- Export only what's necessary (public API)

### 8. Error Handling

- Use custom Error classes for specific errors
- Provide meaningful error messages
- Handle errors at appropriate levels
- Log errors for debugging
- Fail gracefully with fallbacks

## Quality Criteria

- Code follows ES6+ standards and best practices
- All functions are well-documented
- No console errors or warnings
- Asynchronous operations are handled correctly
- DOM manipulation is efficient
- Performance meets standards
- Code is testable and modular
- Passes linting rules (ESLint)

## Example Usage

When building an interactive widget:

1. Structure code into modules
2. Use async/await for data fetching
3. Efficiently query and manipulate DOM
4. Implement event handlers with proper cleanup
5. Optimize performance with debouncing/delegation
6. Add error handling and validation
7. Write unit tests for logic
