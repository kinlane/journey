---
class:
- stop
rel:
- self
properties:
  name: Content-Location (RFC 7231)
  sort: 437
  level: 3
  description: 'The "Content-Location" header field references a URI that can be used
    as an identifier for a specific resource corresponding to the representation in
    this message payload. In other words, if one were to perform a GET request on
    this URI at the time of this message''s generation, then a 200 (OK) response would
    contain the same representation that is enclosed as payload in this message. '
entities:
- class:
  - stop
  rel:
  - self
  properties:
    name: Content-Location (RFC 7231)
  links:
  - rel:
    - self
    href: design/headers/content-location-rfc-7231.md
  - rel:
    - parent
    href: design/headers/
links:
- rel:
  - self
  href: design/headers/content-location-rfc-7231.md
- rel:
  - parent
  href: design/headers/
...
