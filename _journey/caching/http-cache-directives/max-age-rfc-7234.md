---
class:
- stop
rel:
- self
properties:
  name: max-age (RFC 7234)
  sort: 3
  level: 2
  description: 'The "max-age" request directive indicates that the client is unwilling
    to accept a response whose age is greater than the specified number of seconds.
    Unless the max-stale request directive is also present, the client is not willing
    to accept a stale response. The "max-age" response directive indicates that the
    response is to be considered stale after its age is greater than the specified
    number of seconds. '
entities:
- class:
  - stop
  rel:
  - self
  properties:
    name: max-age (RFC 7234)
  links:
  - rel:
    - self
    href: caching/http-cache-directives/max-age-rfc-7234.md
  - rel:
    - parent
    href: caching/http-cache-directives/
links:
- rel:
  - self
  href: caching/http-cache-directives/max-age-rfc-7234.md
- rel:
  - parent
  href: caching/http-cache-directives/
...
