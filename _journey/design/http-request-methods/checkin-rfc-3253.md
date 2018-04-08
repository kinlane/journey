---
class:
- stop
rel:
- self
properties:
  name: CHECKIN (RFC 3253)
  sort: 262
  level: 2
  description: 'A CHECKIN request can be applied to a checked-out version-controlled
    resource to produce a new version whose content and dead properties are copied
    from the checked-out resource. '
entities:
- class:
  - stop
  rel:
  - self
  properties:
    name: CHECKIN (RFC 3253)
  links:
  - rel:
    - self
    href: design/http-request-methods/checkin-rfc-3253.md
  - rel:
    - parent
    href: design/http-request-methods/
links:
- rel:
  - self
  href: design/http-request-methods/checkin-rfc-3253.md
- rel:
  - parent
  href: design/http-request-methods/
...
