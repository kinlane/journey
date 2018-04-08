---
class:
- stop
rel:
- self
properties:
  name: Apply-To-Redirect-Ref (RFC 4437)
  sort: 395
  level: 2
  description: 'The optional Apply-To-Redirect-Ref header can be used on any request
    to a redirect reference resource. When it is present and set to "T", the request
    MUST be applied to the reference resource itself, and a 3xx response MUST NOT
    be returned. '
entities:
- class:
  - stop
  rel:
  - self
  properties:
    name: Apply-To-Redirect-Ref (RFC 4437)
  links:
  - rel:
    - self
    href: design/headers/apply-to-redirect-ref-rfc-4437.md
  - rel:
    - parent
    href: design/headers/
links:
- rel:
  - self
  href: design/headers/apply-to-redirect-ref-rfc-4437.md
- rel:
  - parent
  href: design/headers/
...
