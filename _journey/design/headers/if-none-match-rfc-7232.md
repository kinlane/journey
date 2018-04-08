---
class:
- stop
rel:
- self
properties:
  name: If-None-Match (RFC 7232)
  sort: 517
  level: 2
  description: 'The "If-None-Match" header field makes the request method conditional
    on a recipient cache or origin server either not having any current representation
    of the target resource, when the field-value is "*", or having a selected representation
    with an entity-tag that does not match any of those listed in the field-value. '
entities:
- class:
  - stop
  rel:
  - self
  properties:
    name: If-None-Match (RFC 7232)
  links:
  - rel:
    - self
    href: design/headers/if-none-match-rfc-7232.md
  - rel:
    - parent
    href: design/headers/
links:
- rel:
  - self
  href: design/headers/if-none-match-rfc-7232.md
- rel:
  - parent
  href: design/headers/
...
