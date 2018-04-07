---
class:
- stop
rel:
- self
properties:
  name: On-Premise
  sort: 6
  level: 1
  description: Allowing for on-premise backups to occur, ensuring that backups of
    all resources are available in at least one or two additional locations.
entities:
- class:
  - stop
  rel:
  - self
  properties:
    name: On-Premise
  links:
  - rel:
    - self
    href: backup/on-premise.md
  - rel:
    - parent
    href: backup/
links:
- rel:
  - self
  href: backup/on-premise.md
- rel:
  - parent
  href: backup/
...
