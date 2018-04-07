---
class:
- stop
rel:
- self
properties:
  name: SEARCH (RFC 5323)
  sort: 31
  level: 2
  description: 'The client invokes the SEARCH method to initiate a server-side search.
    The body of the request defines the query. The server MUST emit an entity matching
    the WebDAV multistatus format. '
entities:
- class:
  - stop
  rel:
  - self
  properties:
    name: SEARCH (RFC 5323)
  links:
  - rel:
    - self
    href: design/http-request-methods/search-rfc-5323.md
  - rel:
    - parent
    href: design/http-request-methods/
links:
- rel:
  - self
  href: design/http-request-methods/search-rfc-5323.md
- rel:
  - parent
  href: design/http-request-methods/
...
