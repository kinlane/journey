---
class:
- stop
rel:
- self
properties:
  name: Pragma (RFC 7234)
  sort: 583
  level: 2
  description: 'The "Pragma" header field allows backwards compatibility with HTTP/1.0
    caches, so that clients can specify a "no-cache" request that they will understand
    (as Cache-Control was not defined until HTTP/1.1). When the Cache-Control header
    field is also present and understood in a request, Pragma is ignored. '
entities:
- class:
  - stop
  rel:
  - self
  properties:
    name: Pragma (RFC 7234)
  links:
  - rel:
    - self
    href: design/headers/pragma-rfc-7234.md
  - rel:
    - parent
    href: design/headers/
links:
- rel:
  - self
  href: design/headers/pragma-rfc-7234.md
- rel:
  - parent
  href: design/headers/
...
