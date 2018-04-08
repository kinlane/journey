---
class:
- stop
rel:
- self
properties:
  name: Warning (RFC 7234)
  sort: 695
  level: 2
  description: 'The "Warning" header field is used to carry additional information
    about the status or transformation of a message that might not be reflected in
    the status code. This information is typically used to warn about possible incorrectness
    introduced by caching operations or transformations applied to the payload of
    the message. '
entities:
- class:
  - stop
  rel:
  - self
  properties:
    name: Warning (RFC 7234)
  links:
  - rel:
    - self
    href: design/headers/warning-rfc-7234.md
  - rel:
    - parent
    href: design/headers/
links:
- rel:
  - self
  href: design/headers/warning-rfc-7234.md
- rel:
  - parent
  href: design/headers/
...
