---
class:
- stop
rel:
- self
properties:
  name: Service
  sort: 1100
  level: 3
  description: What 3rd party services are available for delivering proxy services
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
    href: deployment/proxy/service.md
  - rel:
    - parent
    href: deployment/proxy/
links:
- rel:
  - self
  href: deployment/proxy/service.md
- rel:
  - parent
  href: deployment/proxy/
...
