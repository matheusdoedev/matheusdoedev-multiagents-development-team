---
name: relational-databases
description: Workflow for designing and implementing efficient relational database schemas, emphasizing normalization, query optimization, indexing, and transaction management.
keywords: relational databases, SQL, schema design, indexing, query optimization, transactions
---

## Description

This skill provides a workflow for working effectively with relational databases. It emphasizes schema design, query optimization, indexing strategies, and proper transaction management.

## Scope

- Personal skill for backend developers and DBAs
- Applicable to PostgreSQL, MySQL, SQL Server, Oracle
- Can be used for schema design, optimization, and troubleshooting

## Workflow Steps

### 1. Schema Design

- Identify entities and relationships
- Design normalized schemas (3NF minimum)
- Use appropriate data types
- Define primary keys
- Implement foreign keys
- Use constraints appropriately
- Document schema design

### 2. Normalization

- Apply first normal form (1NF)
- Apply second normal form (2NF)
- Apply third normal form (3NF)
- Consider denormalization for performance
- Document deviation from normalization
- Balance normalization with query efficiency
- Review schema for anomalies

### 3. Indexes

- Create indexes on foreign keys
- Index frequently searched columns
- Use composite indexes strategically
- Avoid excessive indexes
- Monitor index effectiveness
- Update statistics
- Use explain plans to verify usage

### 4. Query Optimization

- Write efficient SQL queries
- Avoid N+1 queries
- Use joins appropriately
- Minimize data transfer
- Use appropriate WHERE clauses
- Implement query result caching
- Monitor slow queries

### 5. Transaction Management

- Use appropriate isolation levels
- Implement ACID properties
- Manage connections properly
- Avoid deadlocks
- Use explicit transactions when needed
- Implement retry logic
- Monitor transaction performance

### 6. Data Integrity

- Use foreign key constraints
- Validate data at constraints
- Implement check constraints
- Use unique constraints appropriately
- Maintain referential integrity
- Implement cascading rules
- Document constraints

### 7. Performance Tuning

- Identify bottlenecks
- Use query analysis tools
- Optimize slow queries
- Monitor database metrics
- Implement connection pooling
- Archive old data
- Plan capacity

### 8. Backup and Recovery

- Implement backup strategy
- Test recovery procedures
- Set backup retention
- Monitor backup success
- Document recovery process
- Implement point-in-time recovery
- Plan disaster recovery

## Quality Criteria

- Schema is properly normalized
- Indexes are effective
- Queries perform well
- Data integrity is maintained
- Transactions are handled correctly
- Backups are reliable
- Monitoring is in place
- Documentation is complete

## Common Patterns

### Proper Indexing

- Primary key (clustered index)
- Foreign key indexes
- Composite indexes for common queries
- Partial indexes for filtered data

### Query Optimization

- Use EXPLAIN to analyze queries
- Add indexes for WHERE clauses
- Use appropriate joins
- Minimize columns in SELECT

## Example Usage

When designing a user management database:

1. Create users table with appropriate columns
2. Create indexes on email and username
3. Add foreign keys for relationships
4. Define constraints for data integrity
5. Write optimized queries
6. Monitor query performance
7. Implement backup strategy
