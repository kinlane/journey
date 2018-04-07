---
class:
- stop
rel:
- self
properties:
  name: Connection (RFC 7230)
  sort: 44
  level: 2
  description: 'The "Connection" header field allows the sender to indicate desired
    control options for the current connection. In order to avoid confusing downstream
    recipients, a proxy or gateway MUST remove or replace any received connection
    options before forwarding the message. '
entities:
- class:
  - stop
  rel:
  - self
  properties:
    name: Connection (RFC 7230)
  links:
  - rel:
    - self
    href: design/headers/connection-rfc-7230.md
  - rel:
    - parent
    href: design/headers/
links:
- rel:
  - self
  href: design/headers/connection-rfc-7230.md
- rel:
  - parent
  href: design/headers/
...
