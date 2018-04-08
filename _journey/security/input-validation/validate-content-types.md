---
class:
- stop
rel:
- self
properties:
  name: Validate Content-Types
  sort: 1
  level: 2
  description: The server should never assume the Content-Type; it should always check
    that the Content-Type header and the content are the same type.
entities:
- class:
  - stop
  rel:
  - self
  properties:
    name: Validate Content-Types
  links:
  - rel:
    - self
    href: security/input-validation/validate-content-types.md
  - rel:
    - parent
    href: security/input-validation/
links:
- rel:
  - self
  href: security/input-validation/validate-content-types.md
- rel:
  - parent
  href: security/input-validation/
...
