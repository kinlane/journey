---
class:
- stop
rel:
- self
properties:
  name: Certificates
  sort: 2255
  level: 2
  description: What certificate(s) are in place for protecting a particular service
    to encrypt at all levels of operations.
entities:
- class:
  - stop
  rel:
  - self
  properties:
    name: Certificates
  links:
  - rel:
    - self
    href: encryption/certificates.md
  - rel:
    - parent
    href: encryption/
links:
- rel:
  - self
  href: encryption/certificates.md
- rel:
  - parent
  href: encryption/
...
