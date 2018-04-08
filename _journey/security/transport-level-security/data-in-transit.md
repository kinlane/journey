---
class:
- stop
rel:
- self
properties:
  name: Data in Transit
  sort: 1
  level: 2
  description: Unless the public information is completely read-only, the use of TLS
    should be mandated, particularly where credentials, updates, deletions, and any
    value transactions are performed.
entities:
- class:
  - stop
  rel:
  - self
  properties:
    name: Data in Transit
  links:
  - rel:
    - self
    href: security/transport-level-security/data-in-transit.md
  - rel:
    - parent
    href: security/transport-level-security/
links:
- rel:
  - self
  href: security/transport-level-security/data-in-transit.md
- rel:
  - parent
  href: security/transport-level-security/
...
