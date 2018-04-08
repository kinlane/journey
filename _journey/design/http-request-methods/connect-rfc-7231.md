---
class:
- stop
rel:
- self
properties:
  name: CONNECT (RFC 7231)
  sort: 266
  level: 2
  description: 'The CONNECT method requests that the recipient establish a tunnel
    to the destination origin server identified by the request-target and, if successful,
    thereafter restrict its behavior to blind forwarding of packets, in both directions,
    until the tunnel is closed. Tunnels are commonly used to create an end-to-end
    virtual connection, through one or more proxies, which can then be secured using
    TLS (Transport Layer Security). '
entities:
- class:
  - stop
  rel:
  - self
  properties:
    name: CONNECT (RFC 7231)
  links:
  - rel:
    - self
    href: design/http-request-methods/connect-rfc-7231.md
  - rel:
    - parent
    href: design/http-request-methods/
links:
- rel:
  - self
  href: design/http-request-methods/connect-rfc-7231.md
- rel:
  - parent
  href: design/http-request-methods/
...
