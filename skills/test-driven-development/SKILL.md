---
name: test-driven-development
description: Workflow for practicing Test-Driven Development (TDD), emphasizing writing tests first, iterative development, and using tests to drive design decisions.
keywords: TDD, test-first, iterative development, red-green-refactor, design
---

## Description

This skill provides a workflow for practicing Test-Driven Development. It emphasizes writing tests before implementation, iterative cycles, and using tests to inform design decisions.

## Scope

- Personal skill for developers practicing TDD
- Applicable to any programming language
- Can be used for feature development and refactoring

## Workflow Steps

### 1. Understanding Requirements

- Analyze feature requirements
- Identify acceptance criteria
- Break down into small stories
- Define test cases
- Document expected behavior
- Identify edge cases
- Plan incremental development

### 2. Red Phase - Write Failing Test

- Write a small test for the next feature
- Ensure test fails (red)
- Test should be focused
- Test verifies specific behavior
- Test documents expected API
- Avoid implementation details
- Include assertion for single behavior

### 3. Green Phase - Write Minimal Code

- Write minimal code to pass test
- Code should be simple
- Avoid over-engineering
- Code can be imperfect
- Focus on functionality
- Ignore optimization
- Make test pass with minimal effort

### 4. Refactor Phase - Improve Code

- Refactor code for clarity
- Keep tests passing
- Remove duplication
- Improve design
- Extract methods/functions
- Improve names
- Apply design patterns

### 5. Cycle Repetition

- Repeat red-green-refactor
- Build feature incrementally
- Test drives design
- Emergent design develops
- Code quality improves
- Confidence increases
- Fewer bugs introduced

### 6. Test Organization

- Keep tests focused
- Organize by feature
- Use clear naming
- Document intent
- Maintain test suite
- Run tests frequently
- Keep tests independent

### 7. Design Emergence

- Let tests guide design
- Discover abstractions
- Identify patterns
- Refactor to patterns
- Improve structure
- Reduce coupling
- Improve cohesion

### 8. Collaboration and Feedback

- Discuss test approach with team
- Review test design
- Get feedback on API design
- Discuss refactoring
- Share learnings
- Pair program on complex features
- Document decisions

## Quality Criteria

- Test coverage is high (approaching 100%)
- Code is well-designed
- Code quality is excellent
- Bugs are rare
- Refactoring is confident
- Design is emergent and clean
- Tests document behavior
- Code is maintainable

## Decision Framework

- If test is complex: Design is unclear; simplify test first
- If test is hard to write: API design needs work
- If refactoring is difficult: Code needs better organization
- If test suite is slow: Identify bottlenecks; optimize
- If test fails: Analyze; understand why before fixing

## Example Usage

When implementing a checkout feature:

1. Write test for adding item to cart
2. Implement minimal cart functionality
3. Refactor for clarity
4. Write test for quantity update
5. Implement update functionality
6. Refactor shared logic
7. Continue until feature complete
