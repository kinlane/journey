---
class:
- stop
rel:
- self
properties:
  name: Session State
  sort: 2280
  level: 2
  description: Many web services are written to be as stateless as possible, usually
    ending up with a state blob being sent as part of the transaction.
entities:
- class:
  - stop
  rel:
  - self
  properties:
    name: Session State
  links:
  - rel:
    - self
    href: security/authentication-considerations/session-state.md
  - rel:
    - parent
    href: security/authentication-considerations/
links:
- rel:
  - self
  href: security/authentication-considerations/session-state.md
- rel:
  - parent
  href: security/authentication-considerations/
...
