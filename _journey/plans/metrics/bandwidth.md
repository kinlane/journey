---
class:
- stop
rel:
- self
properties:
  name: Bandwidth
  sort: 20
  level: 2
  description: Measuring API access based upon the amount of bandwidth used.
entities:
- class:
  - stop
  rel:
  - self
  properties:
    name: Bandwidth
  links:
  - rel:
    - self
    href: plans/metrics/bandwidth.md
  - rel:
    - parent
    href: plans/metrics/
links:
- rel:
  - self
  href: plans/metrics/bandwidth.md
- rel:
  - parent
  href: plans/metrics/
...