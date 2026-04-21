---
name: integration-testing
description: Workflow for testing integrated components and systems, emphasizing realistic scenarios, database interactions, API integration, and end-to-end verification.
keywords: integration testing, system testing, database testing, API testing
---

## Description

This skill provides a workflow for writing integration tests that verify multiple components working together. It emphasizes realistic scenarios, data consistency, and system behavior.

## Scope

- Personal skill for backend and full-stack developers
- Applicable to web applications, APIs, and services
- Can be used for testing component interactions and system behavior

## Workflow Steps

### 1. Integration Scope Definition

- Identify components to integrate
- Define integration points
- Plan realistic scenarios
- Document dependencies
- Identify external systems
- Plan test coverage
- Document expected behavior

### 2. Test Environment Setup

- Set up test database
- Configure test data
- Set up mock services
- Configure network settings
- Initialize test fixtures
- Set up cleanup procedures
- Document setup process

### 3. Scenario Testing

- Test end-to-end scenarios
- Verify component communication
- Test data flow between components
- Verify state transitions
- Test error propagation
- Test recovery mechanisms
- Document scenario details

### 4. Database Integration

- Test database interactions
- Verify data persistence
- Test transactions
- Verify data consistency
- Test rollback behavior
- Test concurrent access
- Clean up test data

### 5. API Integration

- Test API endpoints
- Verify request/response handling
- Test authentication
- Test error responses
- Verify data serialization
- Test rate limiting
- Test pagination

### 6. External System Integration

- Mock external systems
- Test API calls
- Verify request format
- Verify response handling
- Test error scenarios
- Test timeouts
- Test retries

### 7. Test Data Management

- Create realistic test data
- Use fixtures
- Seed databases
- Clean up after tests
- Manage test data versions
- Document data assumptions
- Handle data dependencies

### 8. Verification

- Verify correct results
- Verify side effects
- Verify data consistency
- Verify state changes
- Verify error messages
- Verify logging
- Verify performance

## Quality Criteria

- Tests cover critical integrations
- Scenarios are realistic
- Data consistency is verified
- Performance is acceptable
- Tests are maintainable
- Coverage is adequate
- Tests provide confidence
- Debugging information available

## Example Usage

When testing a user registration system:

1. Test form submission end-to-end
2. Verify database persistence
3. Verify email service integration
4. Test error scenarios
5. Verify user creation
6. Test duplicate prevention
7. Verify data consistency
