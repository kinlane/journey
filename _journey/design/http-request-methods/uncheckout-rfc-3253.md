---
class:
- stop
rel:
- self
properties:
  name: UNCHECKOUT (RFC 3253)
  sort: 322
  level: 2
  description: 'An UNCHECKOUT request can be applied to a checked-out version-controlled
    resource to cancel the CHECKOUT and restore the pre-CHECKOUT state of the version-controlled
    resource. '
entities:
- class:
  - stop
  rel:
  - self
  properties:
    name: UNCHECKOUT (RFC 3253)
  links:
  - rel:
    - self
    href: design/http-request-methods/uncheckout-rfc-3253.md
  - rel:
    - parent
    href: design/http-request-methods/
links:
- rel:
  - self
  href: design/http-request-methods/uncheckout-rfc-3253.md
- rel:
  - parent
  href: design/http-request-methods/
...
