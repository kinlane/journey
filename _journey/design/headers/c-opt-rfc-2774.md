---
class:
- stop
rel:
- self
properties:
  name: C-Opt (RFC 2774)
  sort: 407
  level: 3
  description: 'An optional extension declaration indicates that the ultimate recipient
    of the extension MAY consult and adhere to the rules given by the extension when
    processing the message, or ignore the extension declaration completely. An agent
    may not be able to distinguish whether the ultimate recipient does not understand
    an extension referred to by an optional extension or simply ignores the extension
    declaration. Hop-by-hop extension declarations are meaningful only for a single
    HTTP connection. In HTTP/1.1, C-Man, C-Opt, and all header fields with matching
    header-prefix values defined by C-Man and C-Opt MUST be protected by a Connection
    header field. That is, these header fields are to be included as Connection header
    field directives. '
entities:
- class:
  - stop
  rel:
  - self
  properties:
    name: C-Opt (RFC 2774)
  links:
  - rel:
    - self
    href: design/headers/c-opt-rfc-2774.md
  - rel:
    - parent
    href: design/headers/
links:
- rel:
  - self
  href: design/headers/c-opt-rfc-2774.md
- rel:
  - parent
  href: design/headers/
...
