---
class:
- stop
rel:
- self
properties:
  name: Ports
  sort: 3
  level: 1
  description: What ports are in use as part of operating services, including any
    standard and non-standard uses, covering all stages, and environments used as
    part of the platform.
entities:
- class:
  - stop
  rel:
  - self
  properties:
    name: Ports
  links:
  - rel:
    - self
    href: network/ports.md
  - rel:
    - parent
    href: network/
links:
- rel:
  - self
  href: network/ports.md
- rel:
  - parent
  href: network/
...
