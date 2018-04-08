---
class:
- stop
rel:
- self
properties:
  name: MongoDB
  sort: 12
  level: 2
  description: Providing a connection to MongoDB database that allows for quick access
    to tables and fields, making data available through an API from the backend database.
entities:
- class:
  - stop
  rel:
  - self
  properties:
    name: MongoDB
  links:
  - rel:
    - self
    href: deployment/database/mongodb.md
  - rel:
    - parent
    href: deployment/database/
links:
- rel:
  - self
  href: deployment/database/mongodb.md
- rel:
  - parent
  href: deployment/database/
...
