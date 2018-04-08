---
class:
- stop
rel:
- self
properties:
  name: MySQL
  sort: 1024
  level: 2
  description: Providing a connection to MySQL database that allows for quick access
    to tables and fields, making data available through an API from the backend database.
entities:
- class:
  - stop
  rel:
  - self
  properties:
    name: MySQL
  links:
  - rel:
    - self
    href: deployment/database/mysql.md
  - rel:
    - parent
    href: deployment/database/
links:
- rel:
  - self
  href: deployment/database/mysql.md
- rel:
  - parent
  href: deployment/database/
...
