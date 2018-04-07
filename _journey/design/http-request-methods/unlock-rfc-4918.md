---
class:
- stop
rel:
- self
properties:
  name: UNLOCK (RFC 4918)
  sort: 36
  level: 2
  description: 'The UNLOCK method removes the lock identified by the lock token in
    the Lock-Token request header. The Request-URI MUST identify a resource within
    the scope of the lock. '
entities:
- class:
  - stop
  rel:
  - self
  properties:
    name: UNLOCK (RFC 4918)
  links:
  - rel:
    - self
    href: design/http-request-methods/unlock-rfc-4918.md
  - rel:
    - parent
    href: design/http-request-methods/
links:
- rel:
  - self
  href: design/http-request-methods/unlock-rfc-4918.md
- rel:
  - parent
  href: design/http-request-methods/
...
