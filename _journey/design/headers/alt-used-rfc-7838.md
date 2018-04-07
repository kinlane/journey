---
class:
- stop
rel:
- self
properties:
  name: Alt-Used (RFC 7838)
  sort: 28
  level: 2
  description: 'The Alt-Used header field is used in requests to indicate the identity
    of the alternative service in use, just as the Host header field identifies the
    host and port of the origin. Alt-Used is intended to allow alternative services
    to detect loops, differentiate traffic for purposes of load balancing, and generally
    to ensure that it is possible to identify the intended destination of traffic,
    since introducing this information after a protocol is in use has proven to be
    problematic. '
entities:
- class:
  - stop
  rel:
  - self
  properties:
    name: Alt-Used (RFC 7838)
  links:
  - rel:
    - self
    href: design/headers/alt-used-rfc-7838.md
  - rel:
    - parent
    href: design/headers/
links:
- rel:
  - self
  href: design/headers/alt-used-rfc-7838.md
- rel:
  - parent
  href: design/headers/
...
