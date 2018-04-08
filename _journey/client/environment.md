---
class:
- line
rel:
- self
properties:
  name: Environment
  sort: 2773
  level: 2
  description: Brining common definitions of the environments that will be needed
    to work with many different APIs, allowing for a common way to authentication,
    and pass key values to each API being integrated with.
entities:
- class:
  - line
  rel:
  - self
  properties:
    name: Environment
  links:
  - rel:
    - self
    href: client/environment/
  - rel:
    - parent
    href: client/
links:
- rel:
  - self
  href: client/environment/
- rel:
  - parent
  href: client/
...
