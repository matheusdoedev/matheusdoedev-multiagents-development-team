---
name: solid-practices
description: It is a software design skill that gives capabilities to apply SOLID principles to achieve maintainable, flexible, and robust object-oriented designs that adapt to changing requirements.
---

- It is a software design style, where the goal is to write code where components are less coupled to each other.

- It is not a good idea to have a software where the entire application depends of a single component. That makes more difficult to make maintenance, or add more features, because every time I need to make a modification in that component, I must change each component that depend of it.

- Alongside, it is not a good one to have a component that depends of the implementation of another application, instead of depends of the abstract idea (what the component do, instead of how the component do).

- It is a skill that is more use with `object-oriented-programming` paradigm, but the principles can be applied to other paradigms as well, as long as I understand the core idea of each principle and how to apply it in different contexts.

- SOLID is a acronym for five principles:
  - S: Single Responsibility Principle;
  - O: Open-Closed Principle;
  - L: Liskov Substitution Principle;
  - I: Interface Segregation Principle;
  - D: Dependency Inversion Principle.

## Single Responsibility Principle

- Every component in a software should have only one responsibility.
- A component should not be overloaded with multiple responsibilities. That result in a loose coupled software.

## Open-Closed Principle

- Components in a software must be open for extensions, but closed for modifications. In other words, I class must be open for extensions, by using eritance or composition, but closed for modifications, because if I need to modify a class to add a new feature, I can break the existing features.

## Liskov Substitution Principle

-

## Interface Segregation Principle

-

## Dependency Inversion Principle

- The dependency flow must always be towards abstractions insdead of implementations. Components should depend of what a component do and not of how a component do. That makes the software more flexible, because I can change the implementation of a component without change the components that depend of it, as long as I keep the same behavior (what the component do).

- That principle has relation with `hexagonal-architecture` skill, because my dependency flow must flow from more high level abstraction layer to more low level layers, from ports and adapters to the core of the application.
