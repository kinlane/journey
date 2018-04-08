---
class:
- stop
rel:
- self
properties:
  name: PostGres
  sort: 6
  level: 2
  description: Providing a connection to PostGres database that allows for quick access
    to tables and fields, making data available through an API from the backend database.
entities:
- class:
  - stop
  rel:
  - self
  properties:
    name: PostGres
  links:
  - rel:
    - self
    href: deployment/database/postgres.md
  - rel:
    - parent
    href: deployment/database/
links:
- rel:
  - self
  href: deployment/database/postgres.md
- rel:
  - parent
  href: deployment/database/
...
