---
class:
- stop
rel:
- self
properties:
  name: Encryption
  sort: 1863
  level: 2
  description: Applying encryption to all aggregate logging while being stored, and
    in transit, ensuring that no data is leaked at any point in the lifecycle.
entities:
- class:
  - stop
  rel:
  - self
  properties:
    name: Encryption
  links:
  - rel:
    - self
    href: logging/encryption.md
  - rel:
    - parent
    href: logging/
links:
- rel:
  - self
  href: logging/encryption.md
- rel:
  - parent
  href: logging/
...
