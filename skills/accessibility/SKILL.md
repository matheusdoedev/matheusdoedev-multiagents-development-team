---
name: accessibility
description: Workflow for designing and building accessible digital interfaces following WCAG guidelines, emphasizing inclusive design, keyboard navigation, and screen reader support.
keywords: accessibility, WCAG, a11y, inclusive design, keyboard navigation, screen readers
---

## Description

This skill provides a workflow for building accessible interfaces following WCAG 2.1 guidelines. It emphasizes inclusive design, keyboard navigation, screen reader support, and universal access.

## Scope

- Personal skill for all web developers and designers
- Applicable to any web project
- Can be used for design, development, and testing

## Workflow Steps

### 1. Semantic HTML

- Use semantic elements appropriately
- Use proper heading hierarchy
- Use landmark elements
- Use form elements correctly
- Use list elements for lists
- Use button elements for buttons
- Use links for navigation

### 2. Keyboard Navigation

- Ensure all functionality is keyboard accessible
- Implement logical tab order
- Provide skip navigation links
- Test keyboard navigation
- Avoid keyboard traps
- Show focus indicators
- Implement keyboard shortcuts

### 3. Color and Contrast

- Ensure WCAG AA contrast (4.5:1 for text)
- Don't rely on color alone
- Test with colorblind simulators
- Use sufficient contrast for UI components
- Implement high contrast mode support
- Test on different displays
- Document color combinations

### 4. Text and Readability

- Use adequate font sizes
- Use sufficient line height
- Use appropriate line length
- Provide text alternatives for images
- Support text scaling
- Avoid text-only images
- Implement descriptive links

### 5. Screen Reader Support

- Write descriptive alt text
- Use ARIA appropriately
- Announce dynamic content
- Implement proper heading structure
- Use form labels
- Implement landmark roles
- Test with screen readers

### 6. Forms and Input

- Label all form inputs
- Group related inputs
- Provide error messages
- Implement validation feedback
- Support autocomplete
- Use appropriate input types
- Test with accessibility tools

### 7. Multimedia

- Provide captions for video
- Provide transcripts for audio
- Describe visual content
- Provide text alternatives
- Test with various players
- Ensure player accessibility
- Document multimedia content

### 8. Testing and Compliance

- Use accessibility tools (Axe, WAVE)
- Audit with Lighthouse
- Test with screen readers
- Perform keyboard testing
- Test with actual users
- Monitor accessibility
- Fix issues systematically

## Quality Criteria

- Meets WCAG 2.1 Level AA standards
- All content is keyboard accessible
- Design is tested for accessibility
- Screen readers work well
- High contrast mode is supported
- Focus indicators are visible
- Error messages are clear
- Documentation is accessible

## Example Usage

When building a product form:

1. Use semantic form elements
2. Add descriptive labels
3. Ensure keyboard navigation
4. Implement error messages
5. Test color contrast
6. Test with keyboard
7. Test with screen reader
8. Fix any issues found
