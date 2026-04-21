---
name: tailwind-css
description: Workflow for building modern, responsive user interfaces using Tailwind CSS utility-first approach, emphasizing rapid development, component composition, and customization.
keywords: Tailwind CSS, utility-first, responsive design, components, customization
---

## Description

This skill provides a workflow for efficiently building responsive, maintainable UIs using Tailwind CSS. It focuses on utility-first approach, rapid prototyping, component extraction, and customization strategies.

## Scope

- Personal skill for frontend developers using Tailwind CSS
- Applicable to any project using Tailwind (React, Vue, vanilla HTML)
- Can be used for rapid UI development and design system creation

## Workflow Steps

### 1. Tailwind Configuration

- Understand tailwind.config.js structure
- Customize color palette, typography, spacing
- Configure content paths for PurgeCSS
- Add custom utilities and plugins
- Set up dark mode
- Configure responsive breakpoints

### 2. Utility-First Approach

- Compose styles using utility classes
- Build components by combining utilities
- Avoid creating custom CSS unless necessary
- Use responsive prefixes (sm:, md:, lg:)
- Use state variants (hover:, focus:, dark:)
- Leverage arbitrary values [arbitrary-prop]

### 3. Responsive Design

- Use mobile-first breakpoints
- Use responsive prefixes for all screen sizes
- Test on actual devices
- Consider touch targets and spacing
- Use responsive images with aspect ratio
- Implement responsive typography

### 4. Component Extraction

- Extract reusable components using @layer and @apply
- Create component classes for repeated patterns
- Use CSS custom properties for theming
- Keep components flexible and composable
- Document component variants
- Avoid over-engineering single-use components

### 5. Performance Optimization

- Configure PurgeCSS properly
- Use Content configuration correctly
- Minimize CSS file size
- Use production builds
- Lazy load non-critical styles
- Monitor bundle size

### 6. Customization and Theming

- Use Tailwind's extend configuration
- Create custom color schemes
- Implement dark mode variants
- Use CSS custom properties for theming
- Create utility plugins for custom needs
- Document custom utilities

### 7. Accessibility

- Ensure color contrast meets standards
- Use focus states appropriately
- Support reduced-motion preferences
- Ensure keyboard navigation
- Use semantic HTML with Tailwind
- Test with accessibility tools

## Quality Criteria

- UI is responsive and works on all devices
- Tailwind configuration is optimized
- CSS file size is minimal
- Components are reusable and flexible
- Accessibility standards are met
- Performance is optimized
- Code follows consistent patterns

## Example Usage

When building a product card:

1. Use utility classes for layout and spacing
2. Implement responsive design with breakpoints
3. Add hover and state variants
4. Extract to component class if reusable
5. Ensure accessibility with focus states
6. Test on multiple devices
