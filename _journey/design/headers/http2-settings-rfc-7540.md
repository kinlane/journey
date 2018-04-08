---
class:
- stop
rel:
- self
properties:
  name: HTTP2-Settings (RFC 7540)
  sort: 501
  level: 2
  description: 'A request that upgrades from HTTP/1.1 to HTTP/2 MUST include exactly
    one "HTTP2-Settings" header field. The "HTTP2-Settings" header field is a connection-specific
    header field that includes parameters that govern the HTTP/2 connection, provided
    in anticipation of the server accepting the request to upgrade. '
entities:
- class:
  - stop
  rel:
  - self
  properties:
    name: HTTP2-Settings (RFC 7540)
  links:
  - rel:
    - self
    href: design/headers/http2-settings-rfc-7540.md
  - rel:
    - parent
    href: design/headers/
links:
- rel:
  - self
  href: design/headers/http2-settings-rfc-7540.md
- rel:
  - parent
  href: design/headers/
...
