---
class:
- stop
rel:
- self
properties:
  name: Authorization (RFC 7616RFC 5849RFC 7235)
  sort: 401
  level: 2
  description: 'The client is expected to retry the request, passing an Authorization
    header field line with Digest scheme, which is defined according to the framework
    above. The values of the opaque and algorithm fields must be those supplied in
    the WWW-Authenticate response header field for the entity being requested.Protocol
    parameters can be transmitted using the HTTP "Authorization" header field as defined
    by RFC 2617 with the auth-scheme name set to "OAuth" (case insensitive).The "Authorization"
    header field allows a user agent to authenticate itself with an origin server '
entities:
- class:
  - stop
  rel:
  - self
  properties:
    name: Authorization (RFC 7616RFC 5849RFC 7235)
  links:
  - rel:
    - self
    href: design/headers/authorization-rfc-7616rfc-5849rfc-7235.md
  - rel:
    - parent
    href: design/headers/
links:
- rel:
  - self
  href: design/headers/authorization-rfc-7616rfc-5849rfc-7235.md
- rel:
  - parent
  href: design/headers/
...
