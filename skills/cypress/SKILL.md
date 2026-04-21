---
name: cypress
description: Workflow for writing end-to-end tests using Cypress, emphasizing user interactions, visual testing, debugging, and test reliability.
keywords: Cypress, e2e testing, automated testing, user interactions, debugging
---

## Description

This skill provides a workflow for writing reliable end-to-end tests with Cypress. It emphasizes testing user interactions, debugging strategies, and maintaining test reliability.

## Scope

- Personal skill for QA engineers and developers
- Applicable to any web application
- Can be used for e2e testing, CI/CD integration, and quality assurance

## Workflow Steps

### 1. Setup and Configuration

- Install Cypress
- Configure cypress.config.js
- Set up test environment
- Configure base URL
- Set up browser selection
- Enable necessary features

### 2. Test Writing

- Create test files in cypress/e2e/
- Use descriptive test names
- Follow Arrange-Act-Assert pattern
- Write focused tests
- Test user workflows
- Verify UI changes
- Test error handling

### 3. Selectors and Element Queries

- Use cy.get() for element selection
- Use data-testid attributes
- Use semantic selectors
- Avoid brittle selectors
- Use cy.contains() appropriately
- Chain commands effectively
- Handle dynamic content

### 4. User Interactions

- Simulate user actions
- Use cy.type() for text input
- Use cy.click() for clicking
- Use cy.select() for dropdowns
- Use cy.check() for checkboxes
- Test form submission
- Test navigation

### 5. Assertions and Verification

- Assert element visibility
- Assert element content
- Assert element properties
- Assert URL changes
- Assert API responses
- Use cy.intercept() for API mocking
- Implement custom assertions

### 6. Waiting and Timing

- Handle asynchronous operations
- Use cy.intercept() for network requests
- Wait for elements conditionally
- Use .should() for polling
- Avoid hardcoded delays
- Handle slow applications
- Test real-world timing

### 7. Debugging

- Use Cypress debugger
- Use cy.debug() for logging
- Use DevTools integration
- Run tests in headed mode
- Use cypress open for debugging
- Review error messages
- Analyze test failures

### 8. CI/CD Integration

- Configure for CI pipeline
- Run headless tests
- Generate reports
- Implement retries
- Parallel test execution
- Integrate with CI systems
- Monitor test results

## Quality Criteria

- Tests are reliable and not flaky
- Tests are maintainable and understandable
- Tests cover critical user workflows
- Tests run efficiently
- Assertions are meaningful
- Selectors are robust
- Debugging information is available
- Tests work in CI environment

## Example Usage

When testing a login workflow:

1. Visit login page
2. Verify form elements are visible
3. Fill in credentials
4. Submit form
5. Verify successful redirect
6. Verify user is logged in
7. Test error scenarios
