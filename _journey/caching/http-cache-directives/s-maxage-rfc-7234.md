---
class:
- stop
rel:
- self
properties:
  name: s-maxage (RFC 7234)
  sort: 14
  level: 2
  description: 'The "s-maxage" response directive indicates that, in shared caches,
    the maximum age specified by this directive overrides the maximum age specified
    by either the max-age directive or the Expires header field. The s-maxage directive
    also implies the semantics of the proxy-revalidate response directive. '
entities:
- class:
  - stop
  rel:
  - self
  properties:
    name: s-maxage (RFC 7234)
  links:
  - rel:
    - self
    href: caching/http-cache-directives/s-maxage-rfc-7234.md
  - rel:
    - parent
    href: caching/http-cache-directives/
links:
- rel:
  - self
  href: caching/http-cache-directives/s-maxage-rfc-7234.md
- rel:
  - parent
  href: caching/http-cache-directives/
...
