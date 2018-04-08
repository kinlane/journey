---
class:
- stop
rel:
- self
properties:
  name: URI (RFC 2068)
  sort: 673
  level: 2
  description: 'The URI header field has, in past versions of this specification,
    been used as a combination of the existing Location, Content-Location, and Vary
    header fields as well as the future Alternates field. Its primary purpose has
    been to include a list of additional URIs for the resource, including names and
    mirror locations. However, it has become clear that the combination of many different
    functions within this single field has been a barrier to consistently and correctly
    implementing any of those functions. Furthermore, we believe that the identification
    of names and mirror locations would be better performed via the Link header field.
    The URI header field is therefore deprecated in favor of those other fields. '
entities:
- class:
  - stop
  rel:
  - self
  properties:
    name: URI (RFC 2068)
  links:
  - rel:
    - self
    href: design/headers/uri-rfc-2068.md
  - rel:
    - parent
    href: design/headers/
links:
- rel:
  - self
  href: design/headers/uri-rfc-2068.md
- rel:
  - parent
  href: design/headers/
...
