---
class:
- stop
rel:
- self
properties:
  name: SSL
  sort: 1
  level: 2
  description: Transport Layer Security (TLS) and its predecessor, Secure Sockets
    Layer (SSL), both of which are frequently referred to as 'SSL', are cryptographic
    protocols designed to provide communications security over a computer network.
    Always support TLS / SSL by default when it comes to API operations, if at all
    possible.
entities:
- class:
  - stop
  rel:
  - self
  properties:
    name: SSL
  links:
  - rel:
    - self
    href: design/http-requests/ssl.md
  - rel:
    - parent
    href: design/http-requests/
links:
- rel:
  - self
  href: design/http-requests/ssl.md
- rel:
  - parent
  href: design/http-requests/
...
