---
class:
- stop
rel:
- self
properties:
  name: Type
  sort: 3729
  level: 2
  description: Are there custom types of plans available, with a grouping dimension
    that goes beyond just the available plans. Thinking of plan types as a sort of
    categorization, allowing plans to be grouped by other dimensions, for more easily
    sharing with different groups. Think about separate between SaaS, developer, or
    possibly enterprise levels of access, and how plans can be organized by type.
entities:
- class:
  - stop
  rel:
  - self
  properties:
    name: Type
  links:
  - rel:
    - self
    href: plans/elements/type.md
  - rel:
    - parent
    href: plans/elements/
links:
- rel:
  - self
  href: plans/elements/type.md
- rel:
  - parent
  href: plans/elements/
...
