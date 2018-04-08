---
class:
- stop
rel:
- self
properties:
  name: BASELINE-CONTROL (RFC 3253)
  sort: 258
  level: 3
  description: 'A collection can be placed under baseline control with a BASELINE-CONTROL
    request. When a collection is placed under baseline control, the DAV:version-controlled-configuration
    property of the collection is set to identify a new version-controlled configuration.
    This version-controlled configuration can be checked out and then checked in to
    create a new baseline for that collection. '
entities:
- class:
  - stop
  rel:
  - self
  properties:
    name: BASELINE-CONTROL (RFC 3253)
  links:
  - rel:
    - self
    href: design/http-request-methods/baseline-control-rfc-3253.md
  - rel:
    - parent
    href: design/http-request-methods/
links:
- rel:
  - self
  href: design/http-request-methods/baseline-control-rfc-3253.md
- rel:
  - parent
  href: design/http-request-methods/
...
