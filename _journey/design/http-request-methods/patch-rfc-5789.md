---
class:
- stop
rel:
- self
properties:
  name: PATCH (RFC 5789)
  sort: 300
  level: 2
  description: 'The PATCH method requests that a set of changes described in the request
    entity be applied to the resource identified by the Request-URI. The set of changes
    is represented in a format called a "patch document" identified by a media type.
    If the Request-URI does not point to an existing resource, the server MAY create
    a new resource, depending on the patch document type (whether it can logically
    modify a null resource) and permissions, etc. '
entities:
- class:
  - stop
  rel:
  - self
  properties:
    name: PATCH (RFC 5789)
  links:
  - rel:
    - self
    href: design/http-request-methods/patch-rfc-5789.md
  - rel:
    - parent
    href: design/http-request-methods/
links:
- rel:
  - self
  href: design/http-request-methods/patch-rfc-5789.md
- rel:
  - parent
  href: design/http-request-methods/
...
