---
class:
- stop
rel:
- self
properties:
  name: REBIND (RFC 5842)
  sort: 312
  level: 3
  description: 'The REBIND method removes a binding to a resource from a collection,
    and adds a binding to that resource into the collection identified by the Request-URI.
    The request body specifies the binding to be added (segment) and the old binding
    to be removed (href). It is effectively an atomic form of a MOVE request, and
    MUST be treated the same way as MOVE for the purpose of determining access permissions. '
entities:
- class:
  - stop
  rel:
  - self
  properties:
    name: REBIND (RFC 5842)
  links:
  - rel:
    - self
    href: design/http-request-methods/rebind-rfc-5842.md
  - rel:
    - parent
    href: design/http-request-methods/
links:
- rel:
  - self
  href: design/http-request-methods/rebind-rfc-5842.md
- rel:
  - parent
  href: design/http-request-methods/
...
