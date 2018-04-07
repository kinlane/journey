---
class:
- stop
rel:
- self
properties:
  name: Rollback
  sort: 32
  level: 2
  description: Measurement of API accessed based upon the number of rollbacks that
    are executed.
entities:
- class:
  - stop
  rel:
  - self
  properties:
    name: Rollback
  links:
  - rel:
    - self
    href: plans/metrics/rollback.md
  - rel:
    - parent
    href: plans/metrics/
links:
- rel:
  - self
  href: plans/metrics/rollback.md
- rel:
  - parent
  href: plans/metrics/
...
