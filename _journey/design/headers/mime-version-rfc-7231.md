---
class:
- stop
rel:
- self
properties:
  name: MIME-Version (RFC 7231)
  sort: 103
  level: 2
  description: 'HTTP is not a MIME-compliant protocol. However, messages can include
    a single MIME-Version header field to indicate what version of the MIME protocol
    was used to construct the message. Use of the MIME-Version header field indicates
    that the message is in full conformance with the MIME protocol (as defined in
    RFC 2045). Senders are responsible for ensuring full conformance (where possible)
    when exporting HTTP messages to strict MIME environments. '
entities:
- class:
  - stop
  rel:
  - self
  properties:
    name: MIME-Version (RFC 7231)
  links:
  - rel:
    - self
    href: design/headers/mime-version-rfc-7231.md
  - rel:
    - parent
    href: design/headers/
links:
- rel:
  - self
  href: design/headers/mime-version-rfc-7231.md
- rel:
  - parent
  href: design/headers/
...
