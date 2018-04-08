---
class:
- stop
rel:
- self
properties:
  name: TTL (RFC 8030)
  sort: 659
  level: 3
  description: 'An application server MUST include the TTL (Time-To-Live) header field
    in its request for push message delivery. The TTL header field contains a value
    in seconds that suggests how long a push message is retained by the push service. '
entities:
- class:
  - stop
  rel:
  - self
  properties:
    name: TTL (RFC 8030)
  links:
  - rel:
    - self
    href: design/headers/ttl-rfc-8030.md
  - rel:
    - parent
    href: design/headers/
links:
- rel:
  - self
  href: design/headers/ttl-rfc-8030.md
- rel:
  - parent
  href: design/headers/
...
