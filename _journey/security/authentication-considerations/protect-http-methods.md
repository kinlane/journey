---
class:
- stop
rel:
- self
properties:
  name: Protect HTTP Methods
  sort: 4
  level: 2
  description: Making sure the incoming HTTP method is valid for the session token/API
    key and associated resource collection, action, and record.
entities:
- class:
  - stop
  rel:
  - self
  properties:
    name: Protect HTTP Methods
  links:
  - rel:
    - self
    href: security/authentication-considerations/protect-http-methods.md
  - rel:
    - parent
    href: security/authentication-considerations/
links:
- rel:
  - self
  href: security/authentication-considerations/protect-http-methods.md
- rel:
  - parent
  href: security/authentication-considerations/
...