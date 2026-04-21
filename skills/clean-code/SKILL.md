---
name: clean-code
description: It is a skill that provides clean code good practices guidelines. The goal is to use it in order to write maintanable, and reliable code. It can be used to write code, and to review code.
keywords: clean code, code review, refactoring, maintainability, readability
---

This skill provides a comprehensive workflow for writing, reviewing, and refactoring code to adhere to clean code principles. It focuses on readability, maintainability, and simplicity to produce high-quality software.

## Scope

- Personal skill for individual developers
- Applicable to any programming language
- Can be used during coding, code reviews, or refactoring sessions

## Workflow Steps

### 1. Naming Conventions

- Use descriptive, intention-revealing names for variables, functions, and classes
- Avoid abbreviations unless they are widely understood
- Follow language-specific naming conventions (camelCase, snake_case, etc.)

### 2. Function Design

- Keep functions small and focused on a single responsibility
- Limit function parameters to 3 or fewer; use objects for multiple parameters
- Functions should do one thing well and be named accordingly

### 3. Code Structure

- Organize code into logical sections with clear separation of concerns
- Use consistent indentation and formatting
- Avoid deep nesting; consider early returns or guard clauses

### 4. Comments and Documentation

- Write self-documenting code that minimizes the need for comments
- Use comments to explain why, not what
- Keep comments up-to-date with code changes

### 5. Error Handling

- Use exceptions or error codes appropriately for the language
- Avoid silent failures; handle errors explicitly
- Provide meaningful error messages

### 6. Testing

- Write unit tests for all public functions
- Follow TDD principles when possible
- Ensure tests are readable and maintainable

### 7. Code Smells to Avoid

- Duplicated code
- Long methods or classes
- Large parameter lists
- Global state
- Magic numbers

## Quality Criteria

- Code is easily readable by another developer
- Changes can be made with minimal risk of introducing bugs
- Code follows SOLID principles
- Passes all automated tests
- Receives positive feedback in code reviews

## Decision Points

- If code is hard to understand, refactor for clarity
- If a function grows beyond 20 lines, consider splitting it
- If you find duplicated code, extract it into a reusable function
- If tests are failing, prioritize fixing them before adding new features

## Example Usage

When writing new code:

1. Start with a failing test
2. Write the simplest code to pass the test
3. Refactor using the principles above
4. Repeat until all requirements are met

During code review:

1. Check each file against the quality criteria
2. Suggest improvements using the workflow steps
3. Ensure the code follows the project's style guide
