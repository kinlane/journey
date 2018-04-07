---
class:
- stop
rel:
- self
properties:
  name: Alternates (RFC 2295)
  sort: 29
  level: 2
  description: 'The Alternates response header is used to convey the list of variants
    bound to a negotiable resource. This list can also include directives for any
    content negotiation process. If a response from a transparently negotiable resource
    includes an Alternates header, this header MUST contain the complete variant list
    bound to the negotiable resource. Responses from resources which do not support
    transparent content negotiation MAY also use Alternates headers. '
entities:
- class:
  - stop
  rel:
  - self
  properties:
    name: Alternates (RFC 2295)
  links:
  - rel:
    - self
    href: design/headers/alternates-rfc-2295.md
  - rel:
    - parent
    href: design/headers/
links:
- rel:
  - self
  href: design/headers/alternates-rfc-2295.md
- rel:
  - parent
  href: design/headers/
...
