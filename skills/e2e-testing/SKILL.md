---
name: e2e-testing
description: Workflow for designing and implementing end-to-end tests, emphasizing user workflows, test organization, maintenance, and integration with CI/CD pipelines.
keywords: e2e testing, user workflows, automated testing, quality assurance
---

## Description

This skill provides a workflow for designing and implementing comprehensive end-to-end tests. It emphasizes user workflows, test organization, reliability, and CI/CD integration.

## Scope

- Personal skill for QA engineers and developers
- Applicable to web and mobile applications
- Can be used for test planning, implementation, and maintenance

## Workflow Steps

### 1. Test Planning and Design

- Identify critical user workflows
- Define test scenarios
- Prioritize test coverage
- Plan for different browsers/devices
- Document test cases
- Identify edge cases
- Plan maintenance strategy

### 2. Test Environment Setup

- Configure test environment
- Set up test data
- Configure database fixtures
- Set up API mocking
- Configure authentication
- Set up environment variables
- Document setup process

### 3. Test Implementation

- Implement tests for happy paths
- Implement tests for error scenarios
- Use page object model
- Create reusable test utilities
- Organize tests logically
- Use descriptive names
- Document test purpose

### 4. User Interaction Testing

- Test form interactions
- Test navigation flows
- Test keyboard shortcuts
- Test accessibility features
- Test responsive design
- Test multi-step workflows
- Test state transitions

### 5. Data Verification

- Verify UI changes
- Verify data persistence
- Verify API responses
- Verify database state
- Verify error messages
- Verify user feedback
- Verify visual changes

### 6. Test Maintenance

- Update tests when UI changes
- Monitor test failures
- Fix flaky tests
- Refactor test code
- Remove obsolete tests
- Document test updates
- Review test coverage

### 7. Reporting and Monitoring

- Generate test reports
- Track test results
- Monitor test duration
- Implement error tracking
- Analyze failure patterns
- Implement alerting
- Document issues

### 8. CI/CD Integration

- Configure pipeline
- Run tests automatically
- Implement parallel execution
- Set up notifications
- Generate reports
- Track metrics
- Implement retry logic

## Quality Criteria

- Tests cover critical workflows
- Tests are reliable
- Tests run efficiently
- Test maintenance is manageable
- Coverage is adequate
- Tests provide value
- CI/CD integration works
- Test reports are useful

## Example Usage

When planning e2e tests for an e-commerce site:

1. Identify critical workflows (browse, add to cart, checkout)
2. Create test scenarios for each workflow
3. Implement tests with page objects
4. Add data verification
5. Integrate with CI/CD
6. Monitor test results
7. Maintain as application evolves
