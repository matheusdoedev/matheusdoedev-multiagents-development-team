---
name: unit-testing
description: Workflow for writing isolated, focused unit tests that verify individual functions and components, emphasizing mocking, assertions, and test organization.
keywords: unit testing, mocking, assertions, test isolation, testing frameworks
---

## Description

This skill provides a workflow for writing high-quality unit tests. It emphasizes test isolation, clear assertions, effective mocking, and maintainable test code.

## Scope

- Personal skill for all developers
- Applicable to any programming language and framework
- Can be used for test development and code review

## Workflow Steps

### 1. Test Structure and Organization

- Create tests near implementation
- Use clear test file naming
- Organize tests with describe blocks
- Use clear test names
- Follow Arrange-Act-Assert pattern
- Keep tests focused
- Document test purpose

### 2. Test Isolation

- Test single responsibility
- Mock external dependencies
- Avoid test interdependencies
- Reset state between tests
- Use setup and teardown
- Isolate unit from system
- Test behavior, not implementation

### 3. Assertions

- Use appropriate assertions
- Assert on meaningful outcomes
- Verify return values
- Verify side effects
- Verify error conditions
- Implement custom assertions
- Document expected behavior

### 4. Mocking Strategies

- Mock external services
- Use spy functions
- Mock module dependencies
- Create test doubles
- Avoid mocking too much
- Use real objects when appropriate
- Reset mocks between tests

### 5. Test Data

- Create fixtures
- Use test builders
- Minimize test data
- Use meaningful test values
- Avoid magic numbers
- Create reusable test data
- Document test data assumptions

### 6. Coverage

- Measure code coverage
- Test happy paths
- Test error paths
- Test edge cases
- Avoid coverage obsession
- Focus on meaningful coverage
- Use coverage to find gaps

### 7. Performance

- Keep tests fast
- Avoid expensive operations
- Mock time-consuming calls
- Run tests in parallel
- Profile slow tests
- Optimize test database
- Minimize setup overhead

### 8. Maintenance

- Keep tests simple
- Refactor tests regularly
- Update tests with code changes
- Remove obsolete tests
- Review test quality
- Monitor test failures
- Fix flaky tests

## Quality Criteria

- Tests are fast and reliable
- Each test is focused
- Mocks are used appropriately
- Coverage is meaningful
- Tests are maintainable
- No flaky tests
- Tests serve as documentation
- Code quality improved by tests

## Example Usage

When testing a payment calculator:

1. Test basic calculation
2. Test tax calculation
3. Test discount application
4. Test edge cases (zero, negative)
5. Test error conditions
6. Mock external services
7. Verify all paths covered
