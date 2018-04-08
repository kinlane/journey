---
class:
- stop
rel:
- self
properties:
  name: Hybrid
  sort: 7
  level: 1
  description: Allowing for hybrid on-premise and cloud backups to occur, ensuring
    that backups of all resources are available in at least one or two additional
    locations.
  start: 10
  color: 5777D1
  direction: N        
entities:
- class:
  - stop
  rel:
  - self
  properties:
    name: Hybrid
  links:
  - rel:
    - self
    href: backup/hybrid.md
  - rel:
    - parent
    href: backup/
links:
- rel:
  - self
  href: backup/hybrid.md
- rel:
  - parent
  href: backup/
...
