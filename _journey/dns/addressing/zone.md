---
class:
- stop
rel:
- self
properties:
  name: Zone
  sort: 3
  level: 2
  description: Manage the zones for any particular domain.
entities:
- class:
  - stop
  rel:
  - self
  properties:
    name: Zone
  links:
  - rel:
    - self
    href: dns/addressing/zone.md
  - rel:
    - parent
    href: dns/addressing/
links:
- rel:
  - self
  href: dns/addressing/zone.md
- rel:
  - parent
  href: dns/addressing/
...
