---
class:
- stop
rel:
- self
properties:
  name: Accept-Patch (RFC 5789)
  sort: 361
  level: 2
  description: 'This specification introduces a new response header Accept-Patch used
    to specify the patch document formats accepted by the server. Accept-Patch SHOULD
    appear in the OPTIONS response for any resource that supports the use of the PATCH
    method. The presence of the Accept-Patch header in response to any method is an
    implicit indication that PATCH is allowed on the resource identified by the Request-URI. '
entities:
- class:
  - stop
  rel:
  - self
  properties:
    name: Accept-Patch (RFC 5789)
  links:
  - rel:
    - self
    href: design/headers/accept-patch-rfc-5789.md
  - rel:
    - parent
    href: design/headers/
links:
- rel:
  - self
  href: design/headers/accept-patch-rfc-5789.md
- rel:
  - parent
  href: design/headers/
...
