---
class:
- stop
rel:
- self
properties:
  name: SCRAM-SHA-1 (RFC 7804)
  sort: 9
  level: 2
  description: 'HTTP SCRAM is an HTTP Authentication mechanism whose client response
    and server challenge messages are text-based messages containing one or more attribute-value
    pairs separated by commas. SCRAM-SHA-1 is registered for database compatibility
    with implementations of RFC 5802 that want to also expose HTTP access to a related
    service, but it is not recommended for new deployments. '
entities:
- class:
  - stop
  rel:
  - self
  properties:
    name: SCRAM-SHA-1 (RFC 7804)
  links:
  - rel:
    - self
    href: authentication/approaches/scram-sha-1-rfc-7804.md
  - rel:
    - parent
    href: authentication/approaches/
links:
- rel:
  - self
  href: authentication/approaches/scram-sha-1-rfc-7804.md
- rel:
  - parent
  href: authentication/approaches/
...
