---
class:
- stop
rel:
- self
properties:
  name: HEAD (RFC 7231)
  sort: 274
  level: 3
  description: 'The HEAD method is identical to GET except that the server MUST NOT
    send a message body in the response (i.e., the response terminates at the end
    of the header section). The server SHOULD send the same header fields in response
    to a HEAD request as it would have sent if the request had been a GET, except
    that the payload header fields MAY be omitted. This method can be used for obtaining
    metadata about the selected representation without transferring the representation
    data and is often used for testing hypertext links for validity, accessibility,
    and recent modification. '
entities:
- class:
  - stop
  rel:
  - self
  properties:
    name: HEAD (RFC 7231)
  links:
  - rel:
    - self
    href: design/http-request-methods/head-rfc-7231.md
  - rel:
    - parent
    href: design/http-request-methods/
links:
- rel:
  - self
  href: design/http-request-methods/head-rfc-7231.md
- rel:
  - parent
  href: design/http-request-methods/
...
