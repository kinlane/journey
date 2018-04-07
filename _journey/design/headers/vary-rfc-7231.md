---
class:
- stop
rel:
- self
properties:
  name: Vary (RFC 7231)
  sort: 175
  level: 2
  description: 'The "Vary" header field in a response describes what parts of a request
    message, aside from the method, Host header field, and request target, might influence
    the origin server''s process for selecting and representing this response. The
    value consists of either a single asterisk ("*") or a list of header field names
    (case-insensitive). '
entities:
- class:
  - stop
  rel:
  - self
  properties:
    name: Vary (RFC 7231)
  links:
  - rel:
    - self
    href: design/headers/vary-rfc-7231.md
  - rel:
    - parent
    href: design/headers/
links:
- rel:
  - self
  href: design/headers/vary-rfc-7231.md
- rel:
  - parent
  href: design/headers/
...
