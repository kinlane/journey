---
class:
- stop
rel:
- self
properties:
  name: Content-Length (RFC 7230)
  sort: 50
  level: 2
  description: 'When a message does not have a Transfer-Encoding header field, a Content-Length
    header field can provide the anticipated size, as a decimal number of octets,
    for a potential payload body. For messages that do include a payload body, the
    Content-Length field-value provides the framing information necessary for determining
    where the body (and message) ends. For messages that do not include a payload
    body, the Content-Length indicates the size of the selected representation.. '
entities:
- class:
  - stop
  rel:
  - self
  properties:
    name: Content-Length (RFC 7230)
  links:
  - rel:
    - self
    href: design/headers/content-length-rfc-7230.md
  - rel:
    - parent
    href: design/headers/
links:
- rel:
  - self
  href: design/headers/content-length-rfc-7230.md
- rel:
  - parent
  href: design/headers/
...
