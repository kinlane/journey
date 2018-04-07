---
class:
- stop
rel:
- self
properties:
  name: MKCOL (RFC 4918)
  sort: 17
  level: 2
  description: 'MKCOL creates a new collection resource at the location specified
    by the Request-URI. If the Request-URI is already mapped to a resource, then the
    MKCOL MUST fail. During MKCOL processing, a server MUST make the Request-URI an
    internal member of its parent collection, unless the Request-URI is "/". If no
    such ancestor exists, the method MUST fail. When the MKCOL operation creates a
    new collection resource, all ancestors MUST already exist, or the method MUST
    fail with a 409 (Conflict) status code. '
entities:
- class:
  - stop
  rel:
  - self
  properties:
    name: MKCOL (RFC 4918)
  links:
  - rel:
    - self
    href: design/http-request-methods/mkcol-rfc-4918.md
  - rel:
    - parent
    href: design/http-request-methods/
links:
- rel:
  - self
  href: design/http-request-methods/mkcol-rfc-4918.md
- rel:
  - parent
  href: design/http-request-methods/
...
