---
name: html-programming
description: It is skill provides a comprehensive workflow for writing semantic, accessible, and maintainable HTML. It focuses on proper markup structure, accessibility standards (WCAG), performance optimization, and following modern HTML5 conventions..
keywords: semantic HTML, accessibility, maintainability, readability, HTML5
---

## Description

This skill provides a comprehensive workflow for writing semantic, accessible, and maintainable HTML. It focuses on proper markup structure, accessibility standards (WCAG), performance optimization, and following modern HTML5 conventions.

## Scope

- Personal skill for frontend developers and web developers
- Applicable to any HTML5 project
- Can be used during markup creation, code reviews, or accessibility audits

## Workflow Steps

### 1. Semantic Markup Structure

- Use semantic HTML5 elements (header, nav, main, section, article, aside, footer)
- Use correct heading hierarchy (h1, h2, h3, etc.) without skipping levels
- Use list elements (ul, ol, dl) for list content, not divs
- Use form elements (form, fieldset, legend, label) for form markup
- Avoid divitis—use appropriate semantic elements instead of nested divs

### 2. Accessibility (A11y)

- Provide alt text for all images describing their purpose
- Use proper labels for form inputs, buttons, and interactive elements
- Ensure sufficient color contrast (WCAG AA minimum 4.5:1 for text)
- Use aria attributes only when semantic HTML is insufficient
- Test with keyboard navigation and screen readers
- Include skip navigation links for keyboard users

### 3. Meta Information

- Include essential meta tags: charset, viewport, description
- Set appropriate language attribute on html element
- Use meaningful page titles that describe the page content
- Include favicon and apple-touch-icon where appropriate

### 4. Document Structure

- Use a single h1 per page that describes the main topic
- Organize content with proper heading levels
- Use landmarks (header, nav, main, aside, footer) to define page regions
- Separate presentation from structure

### 5. Forms and Input

- Label all form inputs appropriately
- Group related inputs with fieldset and legend
- Use correct input types (email, password, number, date, etc.)
- Provide clear error messages and success feedback
- Mark required fields clearly
- Use placeholders for hints, not labels

### 6. Links and Navigation

- Use descriptive link text ("Learn more about accessibility" not "Click here")
- Indicate external links appropriately
- Use relative URLs for internal links
- Ensure links are keyboard accessible
- Use aria-current for current navigation item

### 7. Media and Embedded Content

- Always provide alt text for images
- Use picture element for responsive images
- Include transcripts for audio content
- Provide captions for video content
- Use video fallbacks for browser compatibility

### 8. Performance Optimization

- Minimize HTML file size
- Defer non-critical CSS and JavaScript loading
- Use semantic elements for better performance
- Lazy load images when appropriate
- Minimize render-blocking resources

## Decision Points

- If content is not interactive: Use semantic elements instead of divs with ARIA
- If implementing tabs or accordions: Use proper ARIA roles or native details/summary
- If content is an image: Provide descriptive alt text, not "image"
- If form is complex: Use fieldsets and legends to group related inputs
- If mobile layout is different: Use responsive meta viewport and media queries

## Quality Criteria

- Page is fully accessible according to WCAG 2.1 Level AA
- Semantic HTML is used appropriately throughout
- All images have meaningful alt text
- Forms are properly labeled and validated
- No keyboard accessibility issues
- Mobile responsive and works on all target browsers
- Passes HTML validation (W3C validator)
- Loading performance is optimized

## Common Elements and Usage

### Structural Elements

- `<header>`: Introductory content, often contains logo and navigation
- `<nav>`: Navigation links, can appear multiple times
- `<main>`: Primary content of the page (one per page)
- `<section>`: Thematic grouping of content
- `<article>`: Self-contained, independent content
- `<aside>`: Related but separate content (sidebars, callouts)
- `<footer>`: Footer content, metadata, related links

### Form Elements

- `<form>`: Container for form controls
- `<fieldset>`: Groups related form controls
- `<legend>`: Caption for fieldset
- `<label>`: Associates text with form input
- `<input type="">`: Various input types with semantic meaning
- `<textarea>`: Multi-line text input
- `<select>`: Dropdown selection

### Interactive Elements

- `<button>`: Clickable button
- `<details>`: Expandable details
- `<summary>`: Summary for details element
- `<dialog>`: Modal dialog

## Example Usage

When building a product listing page:

1. Use semantic structure: header, nav, main with section/article elements
2. Implement proper heading hierarchy starting with h1
3. Add descriptive alt text for product images
4. Create accessible filters using forms with proper labels
5. Include skip navigation link at the top
6. Test keyboard navigation and screen reader compatibility
7. Validate HTML and check accessibility scores
