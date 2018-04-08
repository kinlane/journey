---
class:
- stop
rel:
- self
properties:
  name: MKACTIVITY (RFC 3253)
  sort: 284
  level: 2
  description: 'A MKACTIVITY request creates a new activity resource. A server MAY
    restrict activity creation to particular collections, but a client can determine
    the location of these collections from a DAV:activity-collection-set OPTIONS request. '
entities:
- class:
  - stop
  rel:
  - self
  properties:
    name: MKACTIVITY (RFC 3253)
  links:
  - rel:
    - self
    href: design/http-request-methods/mkactivity-rfc-3253.md
  - rel:
    - parent
    href: design/http-request-methods/
links:
- rel:
  - self
  href: design/http-request-methods/mkactivity-rfc-3253.md
- rel:
  - parent
  href: design/http-request-methods/
...
