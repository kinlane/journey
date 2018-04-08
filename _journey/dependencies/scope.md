---
class:
- stop
rel:
- self
properties:
  name: Scope
  sort: 5
  level: 1
  description: Allow for the definition of different levels of dependencies depending
    on where they are in the service stack, and properly defining the scope of the
    dependency.
entities:
- class:
  - stop
  rel:
  - self
  properties:
    name: Scope
  links:
  - rel:
    - self
    href: dependencies/scope.md
  - rel:
    - parent
    href: dependencies/
links:
- rel:
  - self
  href: dependencies/scope.md
- rel:
  - parent
  href: dependencies/
...
