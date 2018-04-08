---
class:
- stop
rel:
- self
properties:
  name: only-if-cached (RFC 7234)
  sort: 878
  level: 2
  description: 'The "only-if-cached" request directive indicates that the client only
    wishes to obtain a stored response. If it receives this directive, a cache SHOULD
    either respond using a stored response that is consistent with the other constraints
    of the request, or respond with a 504 (Gateway Timeout) status code. If a group
    of caches is being operated as a unified system with good internal connectivity,
    a member cache MAY forward such a request within that group of caches. '
entities:
- class:
  - stop
  rel:
  - self
  properties:
    name: only-if-cached (RFC 7234)
  links:
  - rel:
    - self
    href: caching/http-cache-directives/only-if-cached-rfc-7234.md
  - rel:
    - parent
    href: caching/http-cache-directives/
links:
- rel:
  - self
  href: caching/http-cache-directives/only-if-cached-rfc-7234.md
- rel:
  - parent
  href: caching/http-cache-directives/
...
