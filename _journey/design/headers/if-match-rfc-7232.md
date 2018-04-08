---
class:
- stop
rel:
- self
properties:
  name: If-Match (RFC 7232)
  sort: 513
  level: 2
  description: 'The "If-Match" header field makes the request method conditional on
    the recipient origin server either having at least one current representation
    of the target resource, when the field-value is "*", or having a current representation
    of the target resource that has an entity-tag matching a member of the list of
    entity-tags provided in the field-value. '
entities:
- class:
  - stop
  rel:
  - self
  properties:
    name: If-Match (RFC 7232)
  links:
  - rel:
    - self
    href: design/headers/if-match-rfc-7232.md
  - rel:
    - parent
    href: design/headers/
links:
- rel:
  - self
  href: design/headers/if-match-rfc-7232.md
- rel:
  - parent
  href: design/headers/
...
