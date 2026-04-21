---
name: vite
description: Workflow for building and optimizing projects with Vite build tool, emphasizing fast development experience, module federation, and production optimization.
keywords: Vite, bundler, build tool, dev server, fast development, HMR
---

## Description

This skill provides a workflow for building and optimizing projects using Vite. It emphasizes fast development experience, efficient bundling, and production optimization.

## Scope

- Personal skill for frontend developers
- Applicable to any Vite-supported framework
- Can be used for project setup, configuration, and optimization

## Workflow Steps

### 1. Project Setup

- Create Vite project with create-vite
- Choose appropriate framework template
- Understand project structure
- Configure vite.config.js
- Install dependencies
- Set up development environment

### 2. Development Experience

- Use dev server for fast development
- Leverage Hot Module Replacement (HMR)
- Use import.meta.hot for HMR
- Configure hot reload
- Use environment variables
- Optimize build time

### 3. Module Handling

- Use ES modules throughout project
- Configure module aliases
- Use dynamic imports for code splitting
- Implement lazy loading
- Manage module dependencies
- Optimize module resolution

### 4. Asset Handling

- Optimize image imports
- Use SVG imports effectively
- Configure asset compression
- Handle font loading
- Implement asset versioning
- Use CSS modules

### 5. Build Optimization

- Configure build output
- Implement code splitting strategy
- Optimize chunk sizes
- Use tree-shaking
- Minify code effectively
- Analyze bundle size

### 6. Configuration Management

- Use vite.config.js properly
- Configure plugins
- Set up preprocessing (TypeScript, JSX)
- Configure CSS handling
- Implement custom resolvers
- Use environment-specific configs

### 7. Production Build

- Build for production
- Configure build output directory
- Implement source maps for debugging
- Optimize for performance
- Generate build reports
- Test production build locally

### 8. Deployment

- Configure deployment platform
- Set up CDN for assets
- Implement caching headers
- Monitor performance
- Set up error tracking
- Document deployment process

## Quality Criteria

- Development experience is fast
- Build process is optimized
- Bundle size is minimal
- Code splitting is effective
- Production build works correctly
- Performance metrics meet standards
- Configuration is maintainable
- Deployment is reliable

## Example Usage

When setting up a React project:

1. Create Vite project with React template
2. Configure vite.config.js
3. Set up module aliases
4. Implement code splitting
5. Optimize bundle size
6. Configure deployment
7. Set up monitoring
