---
class:
- stop
rel:
- self
properties:
  name: Public (RFC 2068)
  sort: 127
  level: 2
  description: 'The Public response-header field lists the set of methods supported
    by the server. The purpose of this field is strictly to inform the recipient of
    the capabilities of the server regarding unusual methods. The methods listed may
    or may not be applicable to the Request-URI; the Allow header field MAY be used
    to indicate methods allowed for a particular URI. '
entities:
- class:
  - stop
  rel:
  - self
  properties:
    name: Public (RFC 2068)
  links:
  - rel:
    - self
    href: design/headers/public-rfc-2068.md
  - rel:
    - parent
    href: design/headers/
links:
- rel:
  - self
  href: design/headers/public-rfc-2068.md
- rel:
  - parent
  href: design/headers/
...
