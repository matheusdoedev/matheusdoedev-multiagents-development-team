---
name: nosql-databases
description: Workflow for designing and implementing efficient NoSQL solutions, emphasizing data modeling, scalability, consistency guarantees, and appropriate use cases.
keywords: NoSQL, MongoDB, document databases, data modeling, scalability, consistency
---

## Description

This skill provides a workflow for effectively using NoSQL databases. It emphasizes data modeling for document stores, understanding consistency guarantees, and optimizing for scalability.

## Scope

- Personal skill for backend developers
- Applicable to MongoDB, DynamoDB, Cassandra, and other NoSQL systems
- Can be used for schema design, optimization, and troubleshooting

## Workflow Steps

### 1. NoSQL Database Selection

- Understand database strengths
- Assess consistency needs
- Evaluate scalability requirements
- Consider query patterns
- Compare with relational databases
- Understand CAP theorem implications
- Document choice rationale

### 2. Document Data Modeling

- Design documents for queries
- Avoid deep nesting
- Denormalize strategically
- Use arrays appropriately
- Reference vs. embed decisions
- Design for access patterns
- Document data model

### 3. Indexing Strategy

- Index frequently queried fields
- Use compound indexes
- Understand index overhead
- Monitor index effectiveness
- Remove unused indexes
- Use covering indexes
- Analyze query plans

### 4. Query Patterns

- Understand database query language
- Design queries for performance
- Use aggregation pipelines
- Minimize data transfer
- Use projections
- Implement pagination
- Monitor query performance

### 5. Scalability

- Understand sharding strategy
- Design for horizontal scaling
- Handle shard keys correctly
- Avoid hotspots
- Plan capacity
- Implement caching
- Use read replicas

### 6. Consistency and Transactions

- Understand consistency guarantees
- Use transactions when available
- Handle eventual consistency
- Implement retry logic
- Manage distributed transactions
- Handle conflicts
- Document consistency model

### 7. Data Integrity

- Validate data at application level
- Use schema validation if available
- Implement unique constraints
- Handle referential integrity
- Manage data relationships
- Version documents appropriately
- Document data requirements

### 8. Backup and Recovery

- Implement backup strategy
- Test recovery procedures
- Use point-in-time recovery
- Monitor backup success
- Archive old data
- Implement replication
- Document procedures

## Quality Criteria

- Data model optimizes for queries
- Indexes are effective and necessary
- Queries perform well
- Scalability needs are met
- Data integrity is maintained
- Consistency is appropriate
- Backups are reliable
- Documentation is complete

## Decision Framework

- If queries are complex: Consider relational database
- If scaling horizontally needed: NoSQL may be better
- If strong consistency required: Evaluate options carefully
- If data is highly relational: Relational may be better
- If document structure varies: NoSQL is suitable
- If ACID transactions required: Evaluate support

## Example Usage

When designing a product catalog:

1. Model documents for access patterns
2. Denormalize category information
3. Create indexes on common queries
4. Implement pagination for results
5. Use aggregation for analytics
6. Handle updates efficiently
7. Plan for scalability
