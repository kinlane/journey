---
class:
- stop
rel:
- self
properties:
  name: LABEL (RFC 3253)
  sort: 276
  level: 2
  description: 'A LABEL request can be applied to a version to modify the labels that
    select that version. The case of a label name MUST be preserved when it is stored
    and retrieved. When comparing two label names to decide if they match or not,
    a server SHOULD use a case-sensitive URL-escaped UTF-8 encoded comparison of the
    two label names. '
entities:
- class:
  - stop
  rel:
  - self
  properties:
    name: LABEL (RFC 3253)
  links:
  - rel:
    - self
    href: design/http-request-methods/label-rfc-3253.md
  - rel:
    - parent
    href: design/http-request-methods/
links:
- rel:
  - self
  href: design/http-request-methods/label-rfc-3253.md
- rel:
  - parent
  href: design/http-request-methods/
...
