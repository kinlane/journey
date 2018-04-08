---
class:
- stop
rel:
- self
properties:
  name: Via (RFC 7230)
  sort: 687
  level: 2
  description: 'The "Via" header field indicates the presence of intermediate protocols
    and recipients between the user agent and the server (on requests) or between
    the origin server and the client (on responses), similar to the "Received" header
    field in email (Section 3.6.7 of RFC 5322). Via can be used for tracking message
    forwards, avoiding request loops, and identifying the protocol capabilities of
    senders along the request/response chain. '
entities:
- class:
  - stop
  rel:
  - self
  properties:
    name: Via (RFC 7230)
  links:
  - rel:
    - self
    href: design/headers/via-rfc-7230.md
  - rel:
    - parent
    href: design/headers/
links:
- rel:
  - self
  href: design/headers/via-rfc-7230.md
- rel:
  - parent
  href: design/headers/
...
