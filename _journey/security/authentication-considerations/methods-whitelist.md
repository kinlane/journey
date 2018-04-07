---
class:
- stop
rel:
- self
properties:
  name: Methods Whitelist
  sort: 5
  level: 2
  description: Properly restrict the allowable verbs such that only the allowed verbs
    would work, while all others would return a proper response code (for example,
    a 403 Forbidden).
entities:
- class:
  - stop
  rel:
  - self
  properties:
    name: Methods Whitelist
  links:
  - rel:
    - self
    href: security/authentication-considerations/methods-whitelist.md
  - rel:
    - parent
    href: security/authentication-considerations/
links:
- rel:
  - self
  href: security/authentication-considerations/methods-whitelist.md
- rel:
  - parent
  href: security/authentication-considerations/
...
