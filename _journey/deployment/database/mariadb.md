---
class:
- stop
rel:
- self
properties:
  name: MariaDB
  sort: 1040
  level: 3
  description: Providing a connection to MariaDB database that allows for quick access
    to tables and fields, making data available through an API from the backend database.
entities:
- class:
  - stop
  rel:
  - self
  properties:
    name: MariaDB
  links:
  - rel:
    - self
    href: deployment/database/mariadb.md
  - rel:
    - parent
    href: deployment/database/
links:
- rel:
  - self
  href: deployment/database/mariadb.md
- rel:
  - parent
  href: deployment/database/
...
