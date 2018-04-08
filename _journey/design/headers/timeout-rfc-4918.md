---
class:
- stop
rel:
- self
properties:
  name: Timeout (RFC 4918)
  sort: 661
  level: 3
  description: 'Clients MAY include Timeout request headers in their LOCK requests.
    However, the server is not required to honor or even consider these requests. '
entities:
- class:
  - stop
  rel:
  - self
  properties:
    name: Timeout (RFC 4918)
  links:
  - rel:
    - self
    href: design/headers/timeout-rfc-4918.md
  - rel:
    - parent
    href: design/headers/
links:
- rel:
  - self
  href: design/headers/timeout-rfc-4918.md
- rel:
  - parent
  href: design/headers/
...
