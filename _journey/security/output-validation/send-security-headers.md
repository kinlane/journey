---
class:
- stop
rel:
- self
properties:
  name: Send Security Headers
  sort: 2390
  level: 2
  description: The server should always send the Content-Type header with the correct
    Content-Type, and preferably the Content-Type header should include a charset.
entities:
- class:
  - stop
  rel:
  - self
  properties:
    name: Send Security Headers
  links:
  - rel:
    - self
    href: security/output-validation/send-security-headers.md
  - rel:
    - parent
    href: security/output-validation/
links:
- rel:
  - self
  href: security/output-validation/send-security-headers.md
- rel:
  - parent
  href: security/output-validation/
...
