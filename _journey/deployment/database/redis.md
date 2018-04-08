---
class:
- stop
rel:
- self
properties:
  name: Redis
  sort: 1044
  level: 2
  description: Providing a connection to Redis database that allows for quick access
    to tables and fields, making data available through an API from the backend database.
entities:
- class:
  - stop
  rel:
  - self
  properties:
    name: Redis
  links:
  - rel:
    - self
    href: deployment/database/redis.md
  - rel:
    - parent
    href: deployment/database/
links:
- rel:
  - self
  href: deployment/database/redis.md
- rel:
  - parent
  href: deployment/database/
...
