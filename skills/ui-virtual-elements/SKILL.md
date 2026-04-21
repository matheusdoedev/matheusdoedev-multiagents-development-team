---
name: ui-virtual-elements
description: Workflow for designing effective virtual elements in UI including buttons, forms, dialogs, and interactive components that provide clear feedback and user control.
keywords: UI components, buttons, forms, dialogs, interactive elements, affordance
---

## Description

This skill provides a workflow for designing and implementing effective virtual UI elements. It emphasizes clear affordance, appropriate feedback, and intuitive interaction patterns.

## Scope

- Personal skill for UI/UX designers and frontend developers
- Applicable to web and app interfaces
- Can be used for component design and implementation

## Workflow Steps

### 1. Button Design

- Use clear, descriptive labels
- Indicate button purpose visually
- Distinguish primary from secondary buttons
- Implement hover/focus/active states
- Show loading states
- Provide confirmation for destructive actions
- Ensure accessible size (44x44px minimum)

### 2. Form Elements

- Use appropriate input types
- Implement clear labels
- Show validation state
- Provide helpful error messages
- Implement success feedback
- Support autocomplete
- Test accessibility

### 3. Dialogs and Modals

- Clearly indicate dialog purpose
- Provide close functionality
- Trap focus within dialog
- Implement keyboard navigation
- Provide escape key support
- Show appropriate actions
- Implement overlay appropriately

### 4. Navigation Elements

- Create clear navigation hierarchy
- Show current location
- Implement breadcrumbs when appropriate
- Use consistent styling
- Ensure mobile navigation
- Support keyboard navigation
- Indicate active state

### 5. Feedback and States

- Show loading states
- Implement progress indicators
- Provide success feedback
- Show error states
- Implement disabled states
- Use consistent styling
- Provide clear messages

### 6. Interactive Patterns

- Implement common patterns consistently
- Use recognizable metaphors
- Provide appropriate transitions
- Show state changes
- Implement appropriate animations
- Test on different devices
- Ensure performance

### 7. Accessibility

- Ensure color is not sole indicator
- Provide text alternatives
- Implement keyboard support
- Use semantic HTML
- Test with screen readers
- Support focus management
- Implement proper ARIA

### 8. Testing

- Test interaction patterns
- Test on different devices
- Test with keyboard
- Test with screen readers
- Test accessibility
- Get user feedback
- Iterate based on feedback

## Quality Criteria

- Elements provide clear affordance
- States are obvious
- Interaction is intuitive
- Feedback is immediate
- Accessibility is ensured
- Performance is good
- Design is consistent
- Components are reusable

## Example Usage

When designing a form submission flow:

1. Create form with clear labels
2. Implement validation feedback
3. Add loading state on submit
4. Show success message
5. Handle errors clearly
6. Implement undo if appropriate
7. Ensure keyboard support
