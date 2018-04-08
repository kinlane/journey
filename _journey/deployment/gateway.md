---
class:
- line
rel:
- self
properties:
  name: Gateway
  sort: 6
  level: 2
  description: A heavier duty implementation that provides a doorway to new or existing
    services, providing more robust solutions for accessing backend services via web
    APIs.
entities:
- class:
  - line
  rel:
  - self
  properties:
    name: Gateway
  links:
  - rel:
    - self
    href: deployment/gateway/
  - rel:
    - parent
    href: deployment/
links:
- rel:
  - self
  href: deployment/gateway/
- rel:
  - parent
  href: deployment/
...
