---
class:
- stop
rel:
- self
properties:
  name: Ordering-Type (RFC 3648)
  sort: 563
  level: 3
  description: 'When a collection is created, the client MAY request that it be ordered
    and specify the semantics of the ordering by using the new Ordering-Type header
    with a MKCOL request. For collections that are ordered, the client SHOULD identify
    the semantics of the ordering with a URI in the Ordering-Type header, although
    the client MAY simply set the header value to DAV:custom to indicate that the
    collection is ordered but the semantics of the ordering are not being advertised. '
entities:
- class:
  - stop
  rel:
  - self
  properties:
    name: Ordering-Type (RFC 3648)
  links:
  - rel:
    - self
    href: design/headers/ordering-type-rfc-3648.md
  - rel:
    - parent
    href: design/headers/
links:
- rel:
  - self
  href: design/headers/ordering-type-rfc-3648.md
- rel:
  - parent
  href: design/headers/
...
