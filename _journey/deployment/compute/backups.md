---
class:
- stop
rel:
- self
properties:
  name: Backups
  sort: 9
  level: 2
  description: Enabling the backing up of the compute layer, allowing for easy recovery,
    and scaling from images, but also recurring backup sources.
entities:
- class:
  - stop
  rel:
  - self
  properties:
    name: Backups
  links:
  - rel:
    - self
    href: deployment/compute/backups.md
  - rel:
    - parent
    href: deployment/compute/
links:
- rel:
  - self
  href: deployment/compute/backups.md
- rel:
  - parent
  href: deployment/compute/
...