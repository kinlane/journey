---
class:
- stop
rel:
- self
properties:
  name: Database
  sort: 2
  level: 1
  description: Providing services and tooling for backing up database, allowing for
    easy storage and restore of all database resources.
entities:
- class:
  - stop
  rel:
  - self
  properties:
    name: Database
  links:
  - rel:
    - self
    href: backup/database.md
  - rel:
    - parent
    href: backup/
links:
- rel:
  - self
  href: backup/database.md
- rel:
  - parent
  href: backup/
...
