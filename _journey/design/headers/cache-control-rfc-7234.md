---
class:
- stop
rel:
- self
properties:
  name: Cache-Control (RFC 7234)
  sort: 413
  level: 3
  description: 'The "Cache-Control" header field is used to specify directives for
    caches along the request/response chain. Such cache directives are unidirectional
    in that the presence of a directive in a request does not imply that the same
    directive is to be given in the response. '
entities:
- class:
  - stop
  rel:
  - self
  properties:
    name: Cache-Control (RFC 7234)
  links:
  - rel:
    - self
    href: design/headers/cache-control-rfc-7234.md
  - rel:
    - parent
    href: design/headers/
links:
- rel:
  - self
  href: design/headers/cache-control-rfc-7234.md
- rel:
  - parent
  href: design/headers/
...
