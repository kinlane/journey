---
class:
- stop
rel:
- self
properties:
  name: Accept-Encoding (RFC 7694RFC 7231)
  sort: 9
  level: 2
  description: 'Section 5.3.4 of RFC 7231 defines "Accept-Encoding" as a request header
    field only. This specification expands that definition to allow "Accept-Encoding"
    as a response header field as well. When present in a response, it indicates what
    content codings the resource was willing to accept in the associated request.
    A field value that only contains "identity" implies that no content codings were
    supported.The "Accept-Encoding" header field can be used by user agents to indicate
    what response content-codings are acceptable in the response. An "identity" token
    is used as a synonym for "no encoding" in order to communicate when no encoding
    is preferred. '
entities:
- class:
  - stop
  rel:
  - self
  properties:
    name: Accept-Encoding (RFC 7694RFC 7231)
  links:
  - rel:
    - self
    href: design/headers/accept-encoding-rfc-7694rfc-7231.md
  - rel:
    - parent
    href: design/headers/
links:
- rel:
  - self
  href: design/headers/accept-encoding-rfc-7694rfc-7231.md
- rel:
  - parent
  href: design/headers/
...
