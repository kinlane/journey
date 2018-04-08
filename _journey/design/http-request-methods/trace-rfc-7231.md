---
class:
- stop
rel:
- self
properties:
  name: TRACE (RFC 7231)
  sort: 318
  level: 2
  description: 'The TRACE method requests a remote, application-level loop-back of
    the request message. The final recipient of the request SHOULD reflect the message
    received, excluding some fields described below, back to the client as the message
    body of a 200 (OK) response with a Content-Type of "message/http". The final recipient
    is either the origin server or the first server to receive a Max-Forwards value
    of zero (0) in the request. '
entities:
- class:
  - stop
  rel:
  - self
  properties:
    name: TRACE (RFC 7231)
  links:
  - rel:
    - self
    href: design/http-request-methods/trace-rfc-7231.md
  - rel:
    - parent
    href: design/http-request-methods/
links:
- rel:
  - self
  href: design/http-request-methods/trace-rfc-7231.md
- rel:
  - parent
  href: design/http-request-methods/
...
