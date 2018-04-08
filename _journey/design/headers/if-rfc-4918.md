---
class:
- stop
rel:
- self
properties:
  name: If (RFC 4918)
  sort: 511
  level: 3
  description: 'The If request header is intended to have similar functionality to
    the If-Match header defined in Section 14.24 of RFC 2616. However, the If header
    handles any state token as well as ETags. A typical example of a state token is
    a lock token, and lock tokens are the only state tokens defined in this specification. '
entities:
- class:
  - stop
  rel:
  - self
  properties:
    name: If (RFC 4918)
  links:
  - rel:
    - self
    href: design/headers/if-rfc-4918.md
  - rel:
    - parent
    href: design/headers/
links:
- rel:
  - self
  href: design/headers/if-rfc-4918.md
- rel:
  - parent
  href: design/headers/
...
