---
name: vue
description: Workflow for building responsive applications using Vue.js framework, emphasizing component design, composition, state management, and Vue 3 patterns.
keywords: Vue.js, components, composition API, reactive data, templates
---

## Description

This skill provides a workflow for building applications with Vue.js. It emphasizes component design, the Composition API, reactive data handling, and modern Vue 3 patterns.

## Scope

- Personal skill for Vue developers
- Applicable to Vue 3+
- Can be used for component development, state management, and optimization

## Workflow Steps

### 1. Component Structure

- Use single-file components (.vue files)
- Organize templates, scripts, and styles together
- Use script setup syntax
- Create focused, reusable components
- Use component composition effectively
- Document component props and events

### 2. Templates and Directives

- Use templates for declarative rendering
- Use v-if, v-for, v-show appropriately
- Implement two-way binding with v-model
- Use event handling with @
- Use directives effectively (v-bind, v-on)
- Create custom directives when needed

### 3. Composition API

- Use ref for reactive primitive values
- Use reactive for objects
- Use computed for derived state
- Use watch for side effects
- Implement lifecycle hooks
- Create composables for logic reuse
- Organize code logically with Composition API

### 4. Props and Emits

- Define props with types
- Implement prop validation
- Use emits for child-to-parent communication
- Use v-model for two-way binding
- Document props and events
- Avoid prop mutation

### 5. State Management

- Use local component state with ref/reactive
- Use provide/inject for shared state
- Consider Pinia for complex state
- Implement single source of truth
- Keep state normalized
- Use computed for derived state

### 6. Styling

- Use scoped styles appropriately
- Use CSS modules when needed
- Leverage CSS custom properties
- Use component-specific styles
- Implement dark mode support
- Ensure styles are maintainable

### 7. Performance

- Use v-show for frequent toggling
- Use computed properties for optimization
- Implement code splitting
- Use lazy loading for routes
- Profile with Vue DevTools
- Optimize rendering

### 8. Routing

- Use Vue Router for navigation
- Implement route protection
- Use lazy loading for components
- Handle route parameters
- Implement nested routing
- Manage router state

## Quality Criteria

- Components are well-designed and reusable
- Composition API is used effectively
- Reactive data is handled properly
- Performance is optimized
- Code is maintainable and scalable
- Tests cover component logic
- No console errors or warnings

## Example Usage

When building a product filter:

1. Create Filter and ProductList components
2. Use reactive for filter state
3. Use computed for filtered results
4. Implement watchers for side effects
5. Use emits for communication
6. Add styling with scoped styles
7. Write component tests
