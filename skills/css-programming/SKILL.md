---
name: css-programming
description: A comprehensive workflow for writing maintainable, performant, and scalable CSS. Focuses on modern methodologies (BEM, SMACSS), responsive design, performance optimization, and accessibility considerations.
keywords: CSS, styling, responsive design, maintainability, performance, BEM, SMACSS
---

## Description

This skill provides a comprehensive workflow for writing maintainable, performant, and scalable CSS. It focuses on modern methodologies, responsive design, performance optimization, and accessibility considerations that improve user experience and developer productivity.

## Scope

- Personal skill for frontend developers and web designers
- Applicable to any CSS project (vanilla CSS, preprocessors, CSS-in-JS)
- Can be used during stylesheet creation, code reviews, or performance optimization

## Workflow Steps

### 1. CSS Architecture and Organization

- Use a consistent naming methodology (BEM, SMACSS, or OOCSS)
- Organize stylesheets by component or feature (not by type)
- Keep file sizes manageable; split large stylesheets into modules
- Use a CSS reset or normalize.css to ensure consistency
- Structure files logically: variables/utilities → base styles → components → layouts

### 2. Naming Conventions and Selectors

- Use meaningful, descriptive class names that describe purpose, not appearance
- Avoid overly specific selectors; use low specificity to enable overrides
- Avoid deeply nested selectors (max 3 levels)
- Use semantic naming (e.g., `.button-primary` not `.button-blue`)
- Prefix state classes with `is-` (e.g., `.is-active`, `.is-loading`)
- Use `js-` prefix for JavaScript-targeted classes

### 3. Responsive Design

- Use mobile-first approach; start with mobile styles, enhance for larger screens
- Use relative units (em, rem, %) instead of fixed pixels
- Implement CSS media queries strategically at breakpoints, not per-component
- Use flexible layouts (Flexbox, Grid) instead of fixed positioning
- Test on actual devices and browsers to ensure responsiveness
- Consider touch targets (minimum 44x44 pixels) for mobile

### 4. CSS Variables and Preprocessors

- Use CSS custom properties (variables) for colors, sizes, fonts consistently
- Define variables at :root or component level appropriately
- Use preprocessors (Sass, Less, PostCSS) for mixins, nesting, and compilation if needed
- Keep preprocessor nesting shallow to avoid specificity issues
- Generate minimal, optimized CSS output

### 5. Flexbox and Grid Layouts

- Use Flexbox for one-dimensional layouts (rows or columns)
- Use CSS Grid for two-dimensional layouts
- Prefer modern layout methods over float or positioning
- Test grid layouts at different viewport sizes
- Use gap property for consistent spacing between items

### 6. Typography and Spacing

- Use a consistent type scale (e.g., 1.125 ratio) for heading sizes
- Set base font size on html element (16px is standard)
- Use rem units for sizing and spacing for accessibility
- Maintain consistent line-height (1.5-1.6 for body text)
- Apply appropriate margin/padding consistently across components
- Ensure text is readable: adequate color contrast, font size, line-height

### 7. Colors and Contrast

- Define colors as variables for consistency and maintainability
- Ensure text color contrast meets WCAG AA standards (4.5:1 for normal text)
- Test with color blindness simulators
- Avoid color as sole means of conveying information
- Use CSS filters or color manipulation cautiously for performance

### 8. Performance Optimization

- Minimize CSS file size through tree-shaking and code splitting
- Use production-ready CSS (minified, optimized)
- Avoid @import for stylesheets (use link tags instead)
- Use CSS minification tools
- Avoid expensive properties (box-shadow, filter) in frequently repainted elements
- Use will-change sparingly for animation performance
- Consider critical CSS inlining for above-the-fold content

### 9. Accessibility in CSS

- Ensure text has sufficient contrast
- Don't remove focus styles; style them instead
- Use underlines or other indicators alongside color for links
- Support reduced-motion preferences with prefers-reduced-motion media query
- Ensure interactive elements are keyboard accessible
- Use cursor property appropriately (pointer for buttons, default for text)

### 10. Browser Compatibility and Testing

- Use vendor prefixes only when necessary
- Use autoprefixer to handle cross-browser compatibility
- Test across target browsers and devices
- Use feature queries (@supports) for progressive enhancement
- Gracefully degrade older browser support

## Decision Points

- If styling buttons: Use consistent component-based approach with variants (primary, secondary, disabled)
- If implementing dark mode: Use CSS custom properties to switch themes
- If performance is critical: Profile paint and layout performance, use CSS containment
- If using animations: Prefer transforms and opacity over position changes
- If layout varies significantly: Consider CSS Grid over multiple media queries
- If styling is repetitive: Extract to reusable mixins or utility classes

## Quality Criteria

- CSS is maintainable and easy to update
- Naming follows chosen methodology consistently
- Low specificity (easy to override without !important)
- Responsive and works on all target devices/browsers
- Performance meets standards (Lighthouse score > 90)
- Passes accessibility checks (WCAG AA contrast, keyboard navigation)
- No unused CSS (tree-shaken or cleaned up)
- Code is DRY; no unnecessary repetition

## Common Methodologies

### BEM (Block, Element, Modifier)

```css
.button {
} /* Block */
.button__text {
} /* Element */
.button--primary {
} /* Modifier */
.button--primary.is-active {
} /* State */
```

### Utility-First (Tailwind approach)

```css
.flex {
  display: flex;
}
.m-4 {
  margin: 1rem;
}
.text-lg {
  font-size: 1.125rem;
}
```

### Component-Based

```css
.card {
}
.card-header {
}
.card-body {
}
.card-footer {
}
```

## Example Usage

When styling a navigation component:

1. Define structure in HTML with semantic markup
2. Create CSS class using BEM: `.navbar`, `.navbar__item`, `.navbar--sticky`
3. Use mobile-first approach for responsive styles
4. Implement focus states for keyboard accessibility
5. Use CSS variables for colors and spacing
6. Test on multiple devices and screen sizes
7. Optimize for performance (minify, tree-shake unused styles)
8. Review contrast and accessibility compliance
