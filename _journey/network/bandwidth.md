---
class:
- stop
rel:
- self
properties:
  name: Bandwidth
  sort: 3168
  level: 2
  description: What bandwidth restrictions, costs, and other allowances are in place
    which should be considered, measured, and understood as part of operating services?
entities:
- class:
  - stop
  rel:
  - self
  properties:
    name: Bandwidth
  links:
  - rel:
    - self
    href: network/bandwidth.md
  - rel:
    - parent
    href: network/
links:
- rel:
  - self
  href: network/bandwidth.md
- rel:
  - parent
  href: network/
...
