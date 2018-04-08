---
class:
- stop
rel:
- self
properties:
  name: private (RFC 7234)
  sort: 11
  level: 2
  description: 'The "private" response directive indicates that the response message
    is intended for a single user and MUST NOT be stored by a shared cache. A private
    cache MAY store the response and reuse it for later requests, even if the response
    would normally be non-cacheable. '
entities:
- class:
  - stop
  rel:
  - self
  properties:
    name: private (RFC 7234)
  links:
  - rel:
    - self
    href: caching/http-cache-directives/private-rfc-7234.md
  - rel:
    - parent
    href: caching/http-cache-directives/
links:
- rel:
  - self
  href: caching/http-cache-directives/private-rfc-7234.md
- rel:
  - parent
  href: caching/http-cache-directives/
...
