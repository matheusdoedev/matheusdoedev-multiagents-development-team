---
name: react
description: Workflow for building modern, performant user interfaces using React, emphasizing component architecture, state management, hooks, and best practices for scalable applications.
keywords: React, components, hooks, state management, performance, JSX
---

## Description

This skill provides a workflow for building high-quality applications with React. It emphasizes component design, hooks usage, state management, performance optimization, and modern React patterns.

## Scope

- Personal skill for React developers
- Applicable to React 18+
- Can be used for component development, state management, and optimization

## Workflow Steps

### 1. Component Architecture

- Create small, focused components
- Use function components exclusively
- Implement clear component responsibilities
- Organize components by feature
- Use composition for flexibility
- Create component variants

### 2. JSX and Props

- Use JSX effectively for readable markup
- Pass props for component communication
- Use prop destructuring
- Implement prop validation with TypeScript
- Avoid prop drilling; use context when appropriate
- Document required and optional props

### 3. React Hooks

- Use useState for component state
- Use useEffect for side effects
- Use useContext for global state
- Use useReducer for complex state
- Use custom hooks for logic reuse
- Use useMemo and useCallback for optimization
- Clean up effects properly

### 4. State Management

- Use local component state for UI state
- Use Context API for moderate state sharing
- Consider Redux or Zustand for complex state
- Implement single source of truth
- Keep state normalized
- Update state immutably

### 5. Performance Optimization

- Use React.memo for preventing unnecessary re-renders
- Memoize callbacks with useCallback
- Memoize computations with useMemo
- Use lazy loading for code splitting
- Implement virtual lists for large data
- Profile with React DevTools

### 6. Side Effects and API Integration

- Use useEffect for API calls
- Handle loading and error states
- Cancel requests on cleanup
- Use abort controllers
- Implement proper error handling
- Cache API responses

### 7. Forms

- Use controlled components
- Implement form validation
- Handle form submission
- Use form libraries (React Hook Form) for complex forms
- Display validation errors
- Test form behavior

### 8. Routing

- Use React Router for navigation
- Implement route protection
- Use lazy loading for route components
- Handle route parameters
- Implement nested routing
- Manage route state properly

### 9. Testing

- Write unit tests for components
- Write integration tests
- Mock external dependencies
- Test user interactions
- Use Testing Library for best practices
- Achieve adequate coverage

## Quality Criteria

- Components are small and focused
- State is managed appropriately
- Performance is optimized
- Side effects are handled correctly
- Code is testable and well-tested
- Best practices are followed
- Application is maintainable and scalable
- No console errors or warnings

## Example Usage

When building a todo list application:

1. Create Todo and TodoList components
2. Use useState for todos state
3. Implement useEffect for persistence
4. Add filtering with local state
5. Implement edit and delete functionality
6. Add form for new todos
7. Write component tests
