---
class:
- stop
rel:
- self
properties:
  name: Security-Scheme (RFC 2660)
  sort: 144
  level: 2
  description: 'All S-HTTP compliant agents must generate the Security-Scheme header
    in the headers of all HTTP messages they generate. This header permits other agents
    to detect that they are communicating with an S-HTTP compliant agent and generate
    the appropriate cryptographic options headers. '
entities:
- class:
  - stop
  rel:
  - self
  properties:
    name: Security-Scheme (RFC 2660)
  links:
  - rel:
    - self
    href: design/headers/security-scheme-rfc-2660.md
  - rel:
    - parent
    href: design/headers/
links:
- rel:
  - self
  href: design/headers/security-scheme-rfc-2660.md
- rel:
  - parent
  href: design/headers/
...
