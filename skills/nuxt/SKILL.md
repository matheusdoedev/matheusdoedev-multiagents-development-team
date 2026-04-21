---
name: nuxt
description: Workflow for building full-stack applications with Nuxt.js, emphasizing SSR, file-based routing, composables, and production-ready features for modern web applications.
keywords: Nuxt.js, SSR, full-stack, file-based routing, composables, Vue
---

## Description

This skill provides a workflow for building full-stack applications with Nuxt.js. It emphasizes server-side rendering, file-based routing, composables, server routes, and production deployment.

## Scope

- Personal skill for Nuxt developers
- Applicable to Nuxt 3+
- Can be used for full-stack development, deployment, and optimization

## Workflow Steps

### 1. Project Setup and Configuration

- Create Nuxt project with create-nuxt-app
- Understand nuxt.config.ts configuration
- Configure build and runtime settings
- Set up environment variables
- Install and configure modules
- Set up package dependencies

### 2. File-Based Routing

- Understand app/ directory structure
- Create routes using file conventions
- Implement nested routes
- Handle dynamic routes with [param].vue
- Use optional segments with [[]param].vue
- Implement catch-all routes
- Use route middleware

### 3. Components and Composables

- Create reusable components
- Use auto-import of components
- Create composables for logic sharing
- Use useState for server-client state sharing
- Implement custom hooks
- Use useRouter and useRoute composables

### 4. Server-Side Rendering

- Understand SSR rendering process
- Use useAsyncData for data fetching
- Use useFetch for API calls
- Handle server-side data fetching
- Pass data from server to client
- Implement proper error handling

### 5. API Routes and Server

- Create API routes in server/api/
- Implement RESTful endpoints
- Use middleware for API requests
- Handle authentication in API routes
- Use database connections properly
- Document API endpoints

### 6. Layouts and Pages

- Create layouts in layouts/ directory
- Use NuxtLayout for custom layouts
- Implement nested layouts
- Use definePageMeta for route metadata
- Create pages with meta information
- Implement page transitions

### 7. Modules and Plugins

- Use Nuxt modules for functionality
- Create custom modules
- Use plugins for global functionality
- Register plugins properly
- Use auto-registration when appropriate
- Configure module options

### 8. Build and Deployment

- Configure build settings
- Use static generation when possible
- Configure deployment platform
- Set environment variables for production
- Implement prerendering
- Optimize bundle size

## Quality Criteria

- Project follows Nuxt conventions
- File-based routing is properly structured
- Server-side rendering works correctly
- Data fetching is implemented properly
- API routes are well-designed
- Performance is optimized
- Deployment process is documented
- Code follows best practices

## Example Usage

When building a blog application:

1. Create pages for index and post detail
2. Use useFetch for API data
3. Create Post composable for logic
4. Implement API routes for blog content
5. Use layouts for consistent design
6. Add authentication middleware
7. Deploy with proper SSR configuration
