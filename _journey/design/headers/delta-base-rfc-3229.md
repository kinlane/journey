---
class:
- stop
rel:
- self
properties:
  name: Delta-Base (RFC 3229)
  sort: 471
  level: 3
  description: 'The Delta-Base entity-header field is used in a delta-encoded response
    to specify the entity tag of the base instance. A Delta-Base header field MUST
    be included in a response with an IM header that includes a delta-coding, if the
    request included more than one entity tag in its If-None-Match header field. Any
    response with an IM header that includes a delta-coding MAY include a Delta-Base
    header. '
entities:
- class:
  - stop
  rel:
  - self
  properties:
    name: Delta-Base (RFC 3229)
  links:
  - rel:
    - self
    href: design/headers/delta-base-rfc-3229.md
  - rel:
    - parent
    href: design/headers/
links:
- rel:
  - self
  href: design/headers/delta-base-rfc-3229.md
- rel:
  - parent
  href: design/headers/
...
