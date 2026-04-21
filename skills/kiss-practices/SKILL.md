---
name: kiss-practices
description: Workflow for applying the KISS principle (Keep It Simple, Stupid) to write straightforward, understandable code that solves problems effectively without unnecessary complexity.
keywords: KISS, simplicity, maintainability, straightforward code, clarity
---

## Description

This skill provides a workflow for applying the KISS principle. It emphasizes writing straightforward code, avoiding unnecessary complexity, and prioritizing clarity and understanding.

## Scope

- Personal skill for all developers
- Applicable to all programming languages and domains
- Can be used for code design and review

## Workflow Steps

### 1. Understand the Problem

- Clearly define requirements
- Avoid solving unknown problems
- Don't anticipate future needs
- Ask clarifying questions
- Document assumptions
- Validate understanding
- Identify essential complexity

### 2. Simple Solutions First

- Start with the simplest approach
- Avoid premature optimization
- Don't add frameworks unnecessarily
- Use built-in features first
- Minimize dependencies
- Avoid unnecessary patterns
- Validate the solution works

### 3. Code Clarity

- Use clear variable names
- Use clear function names
- Write self-documenting code
- Avoid clever tricks
- Keep functions focused
- Use meaningful comments
- Make intent obvious

### 4. Avoid Over-Engineering

- Don't build for non-existent requirements
- Don't create unnecessary abstractions
- Avoid excessive modularity
- Don't implement unused features
- Skip "nice to have" features
- Focus on what's needed
- Refactor when needed

### 5. Readable Code

- Use consistent formatting
- Keep indentation shallow
- Avoid deep nesting
- Use descriptive names
- Limit function size
- Minimize cognitive load
- Make code scan-able

### 6. Appropriate Patterns

- Use patterns only when needed
- Don't force patterns
- Document pattern usage
- Consider alternatives
- Evaluate complexity benefit trade-off
- Start simple, add patterns if needed
- Explain complex patterns

### 7. Testing Simplicity

- Test simple scenarios first
- Avoid overly complex tests
- Keep test setup minimal
- Use straightforward assertions
- Test real use cases
- Avoid unnecessary mocking
- Document test intent

### 8. Refactoring Discipline

- Refactor when code becomes unclear
- Remove unused code
- Consolidate duplication
- Simplify complex logic
- Improve naming
- Break into smaller pieces
- Maintain simplicity

## Quality Criteria

- Code is easy to understand
- Solution is straightforward
- No unnecessary complexity
- Dependencies are minimal
- Code is maintainable
- Newcomers understand code quickly
- No premature optimization
- Changes are easy to make

## Decision Framework

- If solution is complex: Simplify or break down
- If multiple approaches exist: Choose the simplest
- If adding pattern: Verify it adds value
- If code is hard to read: Simplify immediately
- If feature isn't needed: Don't implement it
- If dependencies multiply: Re-evaluate necessity

## Anti-Patterns to Avoid

### Over-Engineering

**Problem:** Creating framework for simple problem
**Solution:** Start simple, add complexity only when needed

### Unclear Naming

**Problem:** Cryptic variable names (x, data, temp)
**Solution:** Use clear, descriptive names

### Clever Tricks

**Problem:** Using obscure language features
**Solution:** Prefer straightforward, readable code

### Unnecessary Patterns

**Problem:** Using design pattern for simple code
**Solution:** Apply patterns when complexity warrants

### Premature Optimization

**Problem:** Optimizing before identifying bottlenecks
**Solution:** Profile first, optimize proven issues

## Example Usage

When implementing a simple utility:

1. Define clear requirements
2. Write straightforward solution
3. Use clear variable/function names
4. Avoid unnecessary dependencies
5. Write simple tests
6. Code review for clarity
7. Refactor only if needed
8. Document complex parts
