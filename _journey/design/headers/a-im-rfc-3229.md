---
class:
- stop
rel:
- self
properties:
  name: A-IM (RFC 3229)
  sort: 337
  level: 3
  description: 'The A-IM request-header field is similar to Accept, but restricts
    the instance-manipulations that are acceptable in the response. A response may
    be the result of applying multiple instance-manipulations. When an A-IM request-header
    field includes one or more delta-coding values, the request MUST contain an If-None-Match
    header field, listing one or more entity tags from prior responses for the request-URI. '
entities:
- class:
  - stop
  rel:
  - self
  properties:
    name: A-IM (RFC 3229)
  links:
  - rel:
    - self
    href: design/headers/a-im-rfc-3229.md
  - rel:
    - parent
    href: design/headers/
links:
- rel:
  - self
  href: design/headers/a-im-rfc-3229.md
- rel:
  - parent
  href: design/headers/
...
