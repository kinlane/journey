---
class:
- stop
rel:
- self
properties:
  name: SAP
  sort: 10
  level: 2
  description: Providing a connection to SAP database that allows for quick access
    to tables and fields, making data available through an API from the backend database.
entities:
- class:
  - stop
  rel:
  - self
  properties:
    name: SAP
  links:
  - rel:
    - self
    href: deployment/database/sap.md
  - rel:
    - parent
    href: deployment/database/
links:
- rel:
  - self
  href: deployment/database/sap.md
- rel:
  - parent
  href: deployment/database/
...