---
class:
- stop
rel:
- self
properties:
  name: Upgrade (RFC 7230)
  sort: 675
  level: 2
  description: 'The "Upgrade" header field is intended to provide a simple mechanism
    for transitioning from HTTP/1.1 to some other protocol on the same connection.
    A client MAY send a list of protocols in the Upgrade header field of a request
    to invite the server to switch to one or more of those protocols, in order of
    descending preference, before sending the final response. '
entities:
- class:
  - stop
  rel:
  - self
  properties:
    name: Upgrade (RFC 7230)
  links:
  - rel:
    - self
    href: design/headers/upgrade-rfc-7230.md
  - rel:
    - parent
    href: design/headers/
links:
- rel:
  - self
  href: design/headers/upgrade-rfc-7230.md
- rel:
  - parent
  href: design/headers/
...
