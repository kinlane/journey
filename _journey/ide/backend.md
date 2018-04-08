---
class:
- line
rel:
- self
properties:
  name: Backend
  sort: 2
  level: 2
  description: Providing backend services for development environments allowing for
    the scaling up of jobs, workers, and other elements involved with compiling, working
    with, and executing the services available via a platform.
entities:
- class:
  - line
  rel:
  - self
  properties:
    name: Backend
  links:
  - rel:
    - self
    href: ide/backend/
  - rel:
    - parent
    href: ide/
links:
- rel:
  - self
  href: ide/backend/
- rel:
  - parent
  href: ide/
...
