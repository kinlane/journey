---
class:
- stop
rel:
- self
properties:
  name: WWW-Authenticate (RFC 7616 RFC 7235)
  sort: 691
  level: 3
  description: 'If a server receives a request for an access-protected object, and
    an acceptable Authorization header is not sent, the server responds with a "401
    Unauthorized" status code, and a WWW-Authenticate header as per the framework
    defined above.The "WWW-Authenticate" header field consists of at least one challenge
    that indicates the authentication scheme(s) and parameters applicable to the effective
    request URI. It MUST be included in 401 (Unauthorized) response messages and MAY
    be included in other response messages to indicate that supplying credentials
    (or different credentials) might affect the response. '
entities:
- class:
  - stop
  rel:
  - self
  properties:
    name: WWW-Authenticate (RFC 7616 RFC 7235)
  links:
  - rel:
    - self
    href: design/headers/www-authenticate-rfc-7616-rfc-7235.md
  - rel:
    - parent
    href: design/headers/
links:
- rel:
  - self
  href: design/headers/www-authenticate-rfc-7616-rfc-7235.md
- rel:
  - parent
  href: design/headers/
...
