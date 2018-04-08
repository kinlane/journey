---
class:
- stop
rel:
- self
properties:
  name: Health
  sort: 3920
  level: 2
  description: Factoring in health checks in API consumption, and charging specifically
    on health checks, or changing plans based upon health results.
entities:
- class:
  - stop
  rel:
  - self
  properties:
    name: Health
  links:
  - rel:
    - self
    href: plans/metrics/health.md
  - rel:
    - parent
    href: plans/metrics/
links:
- rel:
  - self
  href: plans/metrics/health.md
- rel:
  - parent
  href: plans/metrics/
...
