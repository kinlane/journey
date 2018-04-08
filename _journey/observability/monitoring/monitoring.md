---
class:
- stop
rel:
- self
properties:
  name: Monitoring
  sort: 2
  level: 2
  description: Actively monitoring and publishing the uptime and availability status
    demonstrates the maturity of platform and makes it more observable.
entities:
- class:
  - stop
  rel:
  - self
  properties:
    name: Monitoring
  links:
  - rel:
    - self
    href: observability/monitoring/monitoring.md
  - rel:
    - parent
    href: observability/monitoring/
links:
- rel:
  - self
  href: observability/monitoring/monitoring.md
- rel:
  - parent
  href: observability/monitoring/
...
