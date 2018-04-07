---
class:
- stop
rel:
- self
properties:
  name: MKWORKSPACE (RFC 3253)
  sort: 19
  level: 2
  description: 'A MKWORKSPACE request creates a new workspace resource. A server MAY
    restrict workspace creation to particular collections, but a client can determine
    the location of these collections from a DAV:workspace-collection-set OPTIONS
    request. '
entities:
- class:
  - stop
  rel:
  - self
  properties:
    name: MKWORKSPACE (RFC 3253)
  links:
  - rel:
    - self
    href: design/http-request-methods/mkworkspace-rfc-3253.md
  - rel:
    - parent
    href: design/http-request-methods/
links:
- rel:
  - self
  href: design/http-request-methods/mkworkspace-rfc-3253.md
- rel:
  - parent
  href: design/http-request-methods/
...
