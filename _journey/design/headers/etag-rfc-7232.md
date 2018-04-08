---
class:
- stop
rel:
- self
properties:
  name: ETag (RFC 7232)
  sort: 485
  level: 2
  description: 'The "ETag" header field in a response provides the current entity-tag
    for the selected representation, as determined at the conclusion of handling the
    request. An entity-tag is an opaque validator for differentiating between multiple
    representations of the same resource, regardless of whether those multiple representations
    are due to resource state changes over time, content negotiation resulting in
    multiple representations being valid at the same time, or both. '
entities:
- class:
  - stop
  rel:
  - self
  properties:
    name: ETag (RFC 7232)
  links:
  - rel:
    - self
    href: design/headers/etag-rfc-7232.md
  - rel:
    - parent
    href: design/headers/
links:
- rel:
  - self
  href: design/headers/etag-rfc-7232.md
- rel:
  - parent
  href: design/headers/
...
