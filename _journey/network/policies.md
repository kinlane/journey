---
class:
- stop
rel:
- self
properties:
  name: Policies
  sort: 5
  level: 1
  description: What network policies are in place, and should be considered as part
    of service operations, making sure behavior is known and sanctioned as part of
    access of to resources.
entities:
- class:
  - stop
  rel:
  - self
  properties:
    name: Policies
  links:
  - rel:
    - self
    href: network/policies.md
  - rel:
    - parent
    href: network/
links:
- rel:
  - self
  href: network/policies.md
- rel:
  - parent
  href: network/
...
