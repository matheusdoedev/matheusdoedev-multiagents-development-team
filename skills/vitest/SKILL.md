---
name: vitest
description: Workflow for writing fast, reliable unit tests using Vitest framework, emphasizing Vite integration, test organization, mocking, and performance.
keywords: Vitest, unit testing, testing framework, mocking, assertions
---

## Description

This skill provides a workflow for writing high-quality unit tests with Vitest. It emphasizes fast test execution, clear test organization, effective mocking, and integration with Vite.

## Scope

- Personal skill for developers writing unit tests
- Applicable to any Vitest-supported project
- Can be used for test development, refactoring, and maintenance

## Workflow Steps

### 1. Setup and Configuration

- Install Vitest in project
- Configure vitest.config.ts
- Set up test environment
- Configure coverage reporting
- Set up IDE integration
- Enable necessary options

### 2. Test Writing

- Create test files in **tests** or .test.ts
- Use describe blocks for organization
- Create focused test cases
- Use clear test names
- Test one thing per test
- Follow Arrange-Act-Assert pattern
- Use meaningful assertions

### 3. Assertions and Matchers

- Use appropriate matchers
- Test return values
- Test error conditions
- Test side effects
- Use snapshot testing carefully
- Implement custom matchers when needed
- Document expected behavior

### 4. Mocking and Stubbing

- Mock external dependencies
- Use vi.mock() for module mocking
- Implement manual mocks
- Use vi.fn() for spy functions
- Mock API calls
- Reset mocks between tests
- Verify mock calls

### 5. Async Testing

- Test async functions with async/await
- Handle Promises correctly
- Test callbacks
- Use beforeEach/afterEach for setup
- Mock timers when needed
- Test timeouts
- Handle race conditions

### 6. Code Coverage

- Run coverage reports
- Aim for meaningful coverage (not just metrics)
- Identify untested code
- Cover edge cases
- Test error paths
- Balance coverage with test value
- Use coverage reports to find gaps

### 7. Test Organization

- Group related tests
- Create test utilities
- Use fixtures for test data
- Share test setup code
- Keep tests independent
- Avoid test interdependencies
- Maintain test readability

### 8. Debugging and Troubleshooting

- Use debugging tools
- Use console logging in tests
- Use debugger statement
- Run single tests
- Run tests in watch mode
- Analyze test failures
- Fix flaky tests

## Quality Criteria

- Tests are fast and reliable
- Tests are well-organized and maintainable
- Code coverage is adequate
- All critical paths are tested
- Mocks are used appropriately
- Tests are independent
- No flaky tests
- Tests serve as documentation

## Example Usage

When testing a utility function:

1. Create test file next to implementation
2. Write test for happy path
3. Write tests for edge cases
4. Write tests for error conditions
5. Implement mocks for dependencies
6. Run coverage report
7. Refine tests as needed
