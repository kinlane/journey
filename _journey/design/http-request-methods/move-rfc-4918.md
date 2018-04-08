---
class:
- stop
rel:
- self
properties:
  name: MOVE (RFC 4918)
  sort: 294
  level: 3
  description: 'The MOVE operation on a non-collection resource is the logical equivalent
    of a copy (COPY), followed by consistency maintenance processing, followed by
    a delete of the source, where all three actions are performed in a single operation.
    The consistency maintenance step allows the server to perform updates caused by
    the move, such as updating all URLs, other than the Request-URI that identifies
    the source resource, to point to the new destination resource. '
entities:
- class:
  - stop
  rel:
  - self
  properties:
    name: MOVE (RFC 4918)
  links:
  - rel:
    - self
    href: design/http-request-methods/move-rfc-4918.md
  - rel:
    - parent
    href: design/http-request-methods/
links:
- rel:
  - self
  href: design/http-request-methods/move-rfc-4918.md
- rel:
  - parent
  href: design/http-request-methods/
...
