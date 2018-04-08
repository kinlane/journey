---
class:
- stop
rel:
- self
properties:
  name: DASL (RFC 5323)
  sort: 461
  level: 3
  description: 'The DASL response header indicates server support for query grammars
    in the OPTIONS method. The value is a list of URIs that indicate the types of
    supported grammars. Note that although the URIs can be used to identify each supported
    search grammar, there is not necessarily a direct relationship between the URI
    and the XML element name that can be used in XML based SEARCH requests (the element
    name itself is identified by its namespace name (a URI reference) and the element''s
    local name). '
entities:
- class:
  - stop
  rel:
  - self
  properties:
    name: DASL (RFC 5323)
  links:
  - rel:
    - self
    href: design/headers/dasl-rfc-5323.md
  - rel:
    - parent
    href: design/headers/
links:
- rel:
  - self
  href: design/headers/dasl-rfc-5323.md
- rel:
  - parent
  href: design/headers/
...
