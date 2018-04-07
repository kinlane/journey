---
class:
- line
rel:
- self
properties:
  name: Error handling
  sort: 7
  level: 2
  description: Going beyond the HTTP status code and making sure there is a plan for
    handling of error codes, and providing consistent behavior when it comes to things
    going wrong in delivering services.
entities:
- class:
  - line
  rel:
  - self
  properties:
    name: Error handling
  links:
  - rel:
    - self
    href: design/error-handling/
  - rel:
    - parent
    href: design/
links:
- rel:
  - self
  href: design/error-handling/
- rel:
  - parent
  href: design/
...
