---
class:
- line
rel:
- self
properties:
  name: Database
  sort: 1
  level: 2
  description: The backend database schema, infrastructure, and other relevant information
    regarding how data is managed, and leveraged to deploy APIs, and deliver the resources
    needed to make the services work.
entities:
- class:
  - line
  rel:
  - self
  properties:
    name: Database
  links:
  - rel:
    - self
    href: deployment/database/
  - rel:
    - parent
    href: deployment/
links:
- rel:
  - self
  href: deployment/database/
- rel:
  - parent
  href: deployment/
...
