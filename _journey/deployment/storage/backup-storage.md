---
class:
- stop
rel:
- self
properties:
  name: Backup Storage
  sort: 1358
  level: 2
  description: Ensuring there is a lower cost storage options for data that won't
    be accessed very often, but should remain available and usable, but at a lower
    rate.
entities:
- class:
  - stop
  rel:
  - self
  properties:
    name: Backup Storage
  links:
  - rel:
    - self
    href: deployment/storage/backup-storage.md
  - rel:
    - parent
    href: deployment/storage/
links:
- rel:
  - self
  href: deployment/storage/backup-storage.md
- rel:
  - parent
  href: deployment/storage/
...
