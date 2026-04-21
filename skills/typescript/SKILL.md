---
name: typescript
description: Workflow for writing type-safe, maintainable code using TypeScript, emphasizing type annotations, interfaces, advanced types, and development best practices.
keywords: TypeScript, type safety, interfaces, generics, decorators, type annotations
---

## Description

This skill provides a workflow for leveraging TypeScript's type system effectively. It focuses on proper type annotations, interface design, advanced types, and patterns that improve code quality and maintainability.

## Scope

- Personal skill for all developers using TypeScript
- Applicable to frontend and backend TypeScript projects
- Can be used for architecture planning and code reviews

## Workflow Steps

### 1. Basic Types and Type Annotations

- Use explicit type annotations for clarity
- Avoid `any` type; use more specific types
- Use union types for multiple possibilities
- Implement literal types for specific values
- Use type aliases effectively
- Understand type inference

### 2. Interfaces and Classes

- Define interfaces for object shapes
- Use interfaces for contracts
- Implement classes with proper types
- Use access modifiers (public, private, protected)
- Implement abstract classes for inheritance
- Use interfaces for composition

### 3. Generics

- Use generics for reusable code
- Create generic functions
- Create generic classes and interfaces
- Use generic constraints appropriately
- Implement conditional types
- Use mapped types for transformations

### 4. Advanced Types

- Use union and intersection types
- Implement discriminated unions
- Use type guards for narrowing
- Implement utility types (Partial, Pick, Omit)
- Use readonly properties
- Implement branded types for validation

### 5. Enums and Constants

- Use enums for related constants
- Prefer const assertions
- Use string enums for debugging
- Avoid numeric enums
- Create const assertions for type safety
- Use object constants as alternatives

### 6. Type Safety

- Enable strict mode in tsconfig.json
- Use strict null checks
- Handle null and undefined properly
- Implement exhaustiveness checking
- Use type guards for runtime safety
- Test type-level code

### 7. Modules and Namespaces

- Use ES6 modules for organization
- Export types and implementations clearly
- Use namespace for organization if needed
- Implement proper re-exports
- Manage module dependencies
- Understand internal vs external types

### 8. Configuration

- Enable strict compiler options
- Configure tsconfig.json appropriately
- Use source maps for debugging
- Set target and module correctly
- Configure declaration files
- Enable type checking in JavaScript files

## Quality Criteria

- Code is fully type-safe with strict mode
- Types are specific and meaningful
- No use of `any` type
- Interfaces define clear contracts
- Generics are used appropriately
- Type errors are resolved before compilation
- Code is maintainable and refactorable
- Tests verify type safety

## Example Usage

When implementing an API client:

1. Define interfaces for API responses
2. Use generics for type-safe requests
3. Create typed request/response models
4. Implement type guards for validation
5. Use advanced types for complex logic
6. Leverage utility types for transformations
7. Enable strict mode for safety
