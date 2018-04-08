---
class:
- stop
rel:
- self
properties:
  name: Safe (RFC 2310)
  sort: 603
  level: 2
  description: 'The Safe response header field is used by origin servers to indicate
    whether repeating the received HTTP request is safe in the sense of Section 9.1.1
    (Safe Methods) of the HTTP/1.1 specification. For the purpose of this specification,
    a HTTP request is considered to be a repetition of a previous request if both
    requests are issued by the same user agent, and apply to the same resource, and
    have the same request method, and both have no request body, or both have request
    bodies which are byte-wise identical after decoding of any content and transfer
    codings. '
entities:
- class:
  - stop
  rel:
  - self
  properties:
    name: Safe (RFC 2310)
  links:
  - rel:
    - self
    href: design/headers/safe-rfc-2310.md
  - rel:
    - parent
    href: design/headers/
links:
- rel:
  - self
  href: design/headers/safe-rfc-2310.md
- rel:
  - parent
  href: design/headers/
...
