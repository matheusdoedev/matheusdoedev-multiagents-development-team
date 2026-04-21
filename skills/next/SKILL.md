---
name: next
description: Workflow for building full-stack applications using Next.js framework, emphasizing file-based routing, API routes, Server Components, data fetching, and deployment.
keywords: Next.js, React, full-stack, SSR, static generation, API routes
---

## Description

This skill provides a workflow for building full-stack applications with Next.js. It emphasizes file-based routing, App Router, Server Components, data fetching, and production deployment.

## Scope

- Personal skill for Next.js developers
- Applicable to Next.js 13+
- Can be used for full-stack development, deployment, and optimization

## Workflow Steps

### 1. Project Setup and Configuration

- Create Next.js project
- Configure next.config.js
- Set up environment variables
- Configure build settings
- Install required dependencies
- Set up development environment

### 2. File-Based Routing

- Understand app/ directory structure
- Create routes with folders
- Implement dynamic routes with [param]
- Use optional segments with [[param]]
- Implement catch-all routes
- Create nested routes
- Implement route groups with (folder)

### 3. Page and Layout Components

- Create pages in app/ directory
- Implement layouts for shared UI
- Use nested layouts
- Create root layout
- Manage metadata with metadata export
- Implement page transitions
- Use error boundaries

### 4. Server Components and Client Components

- Use Server Components by default
- Mark interactive components with 'use client'
- Implement data fetching on server
- Pass data to client components
- Understand rendering strategy
- Optimize for performance
- Handle async operations

### 5. Data Fetching

- Use fetch with revalidate options
- Implement static generation
- Implement incremental static generation (ISR)
- Implement dynamic rendering
- Handle loading states
- Implement error handling
- Cache data appropriately

### 6. API Routes

- Create API routes in app/api/
- Implement REST endpoints
- Handle different HTTP methods
- Implement middleware for APIs
- Use request/response objects
- Handle errors properly
- Document API endpoints

### 7. Middleware and Authentication

- Create middleware for routing
- Implement authentication
- Protect routes with middleware
- Handle session management
- Implement authorization
- Secure API routes
- Handle token refresh

### 8. Deployment and Performance

- Configure deployment platform
- Optimize build size
- Implement caching strategies
- Monitor performance metrics
- Configure CDN
- Set up monitoring
- Implement analytics

## Quality Criteria

- Project follows Next.js conventions
- File-based routing is properly organized
- Server/Client components are used correctly
- Data fetching is optimized
- Performance metrics meet standards
- Security best practices are followed
- Deployment process is documented
- Code is maintainable

## Example Usage

When building an e-commerce application:

1. Create product listing page
2. Implement dynamic product detail pages
3. Create API routes for cart operations
4. Use Server Components for data fetching
5. Implement authentication middleware
6. Create checkout flow
7. Deploy with optimal caching
