---
class:
- stop
rel:
- self
properties:
  name: If-Unmodified-Since (RFC 7232)
  sort: 523
  level: 2
  description: 'The "If-Unmodified-Since" header field makes the request method conditional
    on the selected representation last modification date being earlier than or equal
    to the date provided in the field-value. This field accomplishes the same purpose
    as If-Match for cases where the user agent does not have an entity-tag for the
    representation. '
entities:
- class:
  - stop
  rel:
  - self
  properties:
    name: If-Unmodified-Since (RFC 7232)
  links:
  - rel:
    - self
    href: design/headers/if-unmodified-since-rfc-7232.md
  - rel:
    - parent
    href: design/headers/
links:
- rel:
  - self
  href: design/headers/if-unmodified-since-rfc-7232.md
- rel:
  - parent
  href: design/headers/
...
