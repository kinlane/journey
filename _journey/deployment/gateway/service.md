---
class:
- stop
rel:
- self
properties:
  name: Service
  sort: 4
  level: 2
  description: What 3rd party services are available for delivering gateway services
    in association with a platform's operation, providing a sanctioned commercial
    service.
entities:
- class:
  - stop
  rel:
  - self
  properties:
    name: Service
  links:
  - rel:
    - self
    href: deployment/gateway/service.md
  - rel:
    - parent
    href: deployment/gateway/
links:
- rel:
  - self
  href: deployment/gateway/service.md
- rel:
  - parent
  href: deployment/gateway/
...
