---
class:
- stop
rel:
- self
properties:
  name: Label (RFC 3253)
  sort: 527
  level: 2
  description: 'For certain methods (e.g. GET, PROPFIND), if the request-URL identifies
    a version-controlled resource, a label can be specified in a Label request header
    to cause the method to be applied to the version selected by that label from the
    version history of that version-controlled resource. '
entities:
- class:
  - stop
  rel:
  - self
  properties:
    name: Label (RFC 3253)
  links:
  - rel:
    - self
    href: design/headers/label-rfc-3253.md
  - rel:
    - parent
    href: design/headers/
links:
- rel:
  - self
  href: design/headers/label-rfc-3253.md
- rel:
  - parent
  href: design/headers/
...
