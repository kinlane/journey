---
class:
- stop
rel:
- self
properties:
  name: Trailer (RFC 7230)
  sort: 667
  level: 2
  description: 'When a message includes a message body encoded with the chunked transfer
    coding and the sender desires to send metadata in the form of trailer fields at
    the end of the message, the sender SHOULD generate a Trailer header field before
    the message body to indicate which fields will be present in the trailers. '
entities:
- class:
  - stop
  rel:
  - self
  properties:
    name: Trailer (RFC 7230)
  links:
  - rel:
    - self
    href: design/headers/trailer-rfc-7230.md
  - rel:
    - parent
    href: design/headers/
links:
- rel:
  - self
  href: design/headers/trailer-rfc-7230.md
- rel:
  - parent
  href: design/headers/
...
