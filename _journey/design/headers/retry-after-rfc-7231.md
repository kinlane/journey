---
class:
- stop
rel:
- self
properties:
  name: Retry-After (RFC 7231)
  sort: 132
  level: 2
  description: 'Servers send the "Retry-After" header field to indicate how long the
    user agent ought to wait before making a follow-up request. When sent with a 503
    (Service Unavailable) response, Retry-After indicates how long the service is
    expected to be unavailable to the client. When sent with any 3xx (Redirection)
    response, Retry-After indicates the minimum time that the user agent is asked
    to wait before issuing the redirected request. '
entities:
- class:
  - stop
  rel:
  - self
  properties:
    name: Retry-After (RFC 7231)
  links:
  - rel:
    - self
    href: design/headers/retry-after-rfc-7231.md
  - rel:
    - parent
    href: design/headers/
links:
- rel:
  - self
  href: design/headers/retry-after-rfc-7231.md
- rel:
  - parent
  href: design/headers/
...
