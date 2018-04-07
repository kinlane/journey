---
class:
- stop
rel:
- self
properties:
  name: max-stale (RFC 7234)
  sort: 4
  level: 2
  description: 'The "max-stale" request directive indicates that the client is willing
    to accept a response that has exceeded its freshness lifetime. If max-stale is
    assigned a value, then the client is willing to accept a response that has exceeded
    its freshness lifetime by no more than the specified number of seconds. If no
    value is assigned to max-stale, then the client is willing to accept a stale response
    of any age. '
entities:
- class:
  - stop
  rel:
  - self
  properties:
    name: max-stale (RFC 7234)
  links:
  - rel:
    - self
    href: caching/http-cache-directives/max-stale-rfc-7234.md
  - rel:
    - parent
    href: caching/http-cache-directives/
links:
- rel:
  - self
  href: caching/http-cache-directives/max-stale-rfc-7234.md
- rel:
  - parent
  href: caching/http-cache-directives/
...
