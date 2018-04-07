---
class:
- stop
rel:
- self
properties:
  name: ALPN (RFC 7639)
  sort: 2
  level: 2
  description: 'Clients include the ALPN header field in an HTTP CONNECT request to
    indicate the application-layer protocol that a client intends to use within the
    tunnel, or a set of protocols that might be used within the tunnel. '
entities:
- class:
  - stop
  rel:
  - self
  properties:
    name: ALPN (RFC 7639)
  links:
  - rel:
    - self
    href: design/headers/alpn-rfc-7639.md
  - rel:
    - parent
    href: design/headers/
links:
- rel:
  - self
  href: design/headers/alpn-rfc-7639.md
- rel:
  - parent
  href: design/headers/
...
