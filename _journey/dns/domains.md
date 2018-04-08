---
class:
- line
rel:
- self
properties:
  name: Domain(s)
  sort: 926
  level: 2
  description: Details regarding what domains are available for making available for
    service deployment, allowing for consistent, and meaningful addressing and deployment
    of services.
entities:
- class:
  - line
  rel:
  - self
  properties:
    name: Domain(s)
  links:
  - rel:
    - self
    href: dns/domains/
  - rel:
    - parent
    href: dns/
links:
- rel:
  - self
  href: dns/domains/
- rel:
  - parent
  href: dns/
...
