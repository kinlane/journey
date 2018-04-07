---
class:
- stop
rel:
- self
properties:
  name: no-store (RFC 7234)
  sort: 8
  level: 2
  description: 'The "no-store" directive indicates that a cache MUST NOT store any
    part of either this request or any response to it. This directive applies to both
    private and shared caches. "MUST NOT store" in this context means that the cache
    MUST NOT intentionally store the information in non-volatile storage, and MUST
    make a best-effort attempt to remove the information from volatile storage as
    promptly as possible after forwarding it. '
entities:
- class:
  - stop
  rel:
  - self
  properties:
    name: no-store (RFC 7234)
  links:
  - rel:
    - self
    href: caching/http-cache-directives/no-store-rfc-7234.md
  - rel:
    - parent
    href: caching/http-cache-directives/
links:
- rel:
  - self
  href: caching/http-cache-directives/no-store-rfc-7234.md
- rel:
  - parent
  href: caching/http-cache-directives/
...
