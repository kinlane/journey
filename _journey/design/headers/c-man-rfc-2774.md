---
class:
- stop
rel:
- self
properties:
  name: C-Man (RFC 2774)
  sort: 35
  level: 2
  description: 'A mandatory extension declaration indicates that the ultimate recipient
    MUST consult and adhere to the rules given by the extension when processing the
    message or reporting an error. Hop-by-hop extension declarations are meaningful
    only for a single HTTP connection. In HTTP/1.1, C-Man, C-Opt, and all header fields
    with matching header-prefix values defined by C-Man and C-Opt MUST be protected
    by a Connection header field. That is, these header fields are to be included
    as Connection header field directives. '
entities:
- class:
  - stop
  rel:
  - self
  properties:
    name: C-Man (RFC 2774)
  links:
  - rel:
    - self
    href: design/headers/c-man-rfc-2774.md
  - rel:
    - parent
    href: design/headers/
links:
- rel:
  - self
  href: design/headers/c-man-rfc-2774.md
- rel:
  - parent
  href: design/headers/
...
