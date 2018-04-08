---
class:
- stop
rel:
- self
properties:
  name: min-fresh (RFC 7234)
  sort: 5
  level: 2
  description: 'The "min-fresh" request directive indicates that the client is willing
    to accept a response whose freshness lifetime is no less than its current age
    plus the specified time in seconds. That is, the client wants a response that
    will still be fresh for at least the specified number of seconds. '
entities:
- class:
  - stop
  rel:
  - self
  properties:
    name: min-fresh (RFC 7234)
  links:
  - rel:
    - self
    href: caching/http-cache-directives/min-fresh-rfc-7234.md
  - rel:
    - parent
    href: caching/http-cache-directives/
links:
- rel:
  - self
  href: caching/http-cache-directives/min-fresh-rfc-7234.md
- rel:
  - parent
  href: caching/http-cache-directives/
...
