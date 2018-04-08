---
class:
- stop
rel:
- self
properties:
  name: no-cache (RFC 7234)
  sort: 7
  level: 2
  description: 'The "no-cache" request directive indicates that a cache MUST NOT use
    a stored response to satisfy the request without successful validation on the
    origin server. The "no-cache" response directive indicates that the response MUST
    NOT be used to satisfy a subsequent request without successful validation on the
    origin server. This allows an origin server to prevent a cache from using it to
    satisfy a request without contacting it, even by caches that have been configured
    to send stale responses. '
entities:
- class:
  - stop
  rel:
  - self
  properties:
    name: no-cache (RFC 7234)
  links:
  - rel:
    - self
    href: caching/http-cache-directives/no-cache-rfc-7234.md
  - rel:
    - parent
    href: caching/http-cache-directives/
links:
- rel:
  - self
  href: caching/http-cache-directives/no-cache-rfc-7234.md
- rel:
  - parent
  href: caching/http-cache-directives/
...
