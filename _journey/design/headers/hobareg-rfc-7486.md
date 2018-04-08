---
class:
- stop
rel:
- self
properties:
  name: Hobareg (RFC 7486)
  sort: 505
  level: 3
  description: 'The server MUST add a header field to the response message when the
    registration has succeeded in order to indicate the new state. The header to be
    used is "Hobareg", and the value when registration has succeeded is to be "regok".
    When registration is in an intermediate state (e.g., on an HTTP response for an
    interstitial page), the server MAY add this header with a value of "reginwork". '
entities:
- class:
  - stop
  rel:
  - self
  properties:
    name: Hobareg (RFC 7486)
  links:
  - rel:
    - self
    href: design/headers/hobareg-rfc-7486.md
  - rel:
    - parent
    href: design/headers/
links:
- rel:
  - self
  href: design/headers/hobareg-rfc-7486.md
- rel:
  - parent
  href: design/headers/
...
