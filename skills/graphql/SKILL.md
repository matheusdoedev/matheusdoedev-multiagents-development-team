---
name: graphql
description: Workflow for designing and implementing GraphQL APIs, emphasizing schema design, resolvers, data loaders, and best practices for efficient querying and type safety.
keywords: GraphQL, API design, schema, resolvers, queries, mutations, subscriptions
---

## Description

This skill provides a workflow for building GraphQL APIs. It emphasizes schema design, resolver implementation, performance optimization, and best practices for type-safe APIs.

## Scope

- Personal skill for backend developers building GraphQL APIs
- Applicable to Apollo Server, GraphQL Yoga, and other implementations
- Can be used for API design, optimization, and client integration

## Workflow Steps

### 1. Schema Design

- Define types that represent domain entities
- Use appropriate scalar types
- Implement relationships between types
- Create input types for mutations
- Use enums for fixed values
- Document schema with descriptions
- Design schema for versioning

### 2. Queries

- Create root Query type
- Implement single item queries
- Implement list queries with filtering
- Support pagination
- Implement search functionality
- Use aliases for flexibility
- Design queries for client needs

### 3. Mutations

- Create root Mutation type
- Implement create operations
- Implement update operations
- Implement delete operations
- Return meaningful responses
- Handle validation errors
- Implement proper error codes

### 4. Subscriptions

- Implement real-time subscriptions
- Use pub/sub for events
- Handle subscription cleanup
- Implement proper error handling
- Test subscription behavior
- Monitor subscription connections

### 5. Resolvers

- Implement efficient resolvers
- Return correct types from resolvers
- Handle null values appropriately
- Implement proper error handling
- Use context for shared data
- Implement data loaders for optimization

### 6. Performance Optimization

- Use DataLoaders to prevent N+1 queries
- Implement query depth limiting
- Use caching strategies
- Batch database queries
- Implement field-level permissions
- Monitor query performance

### 7. Authentication and Authorization

- Implement authentication in context
- Check authorization in resolvers
- Implement field-level permissions
- Use directives for authorization
- Secure sensitive mutations
- Handle token expiration

### 8. Testing

- Write tests for queries
- Write tests for mutations
- Write tests for resolvers
- Mock data sources
- Test error scenarios
- Test pagination and filtering

## Quality Criteria

- Schema is well-designed and documented
- Resolvers are efficient
- Queries perform well
- Error handling is comprehensive
- Security best practices are followed
- API is tested thoroughly
- Documentation is clear
- Type safety is maintained

## Example Usage

When building a product API:

1. Define Product type with fields
2. Create Query for products and product by ID
3. Create Mutation for create/update/delete
4. Implement efficient resolvers
5. Use DataLoaders for relationships
6. Add authentication middleware
7. Write comprehensive tests
