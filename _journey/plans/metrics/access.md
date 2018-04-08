---
class:
- stop
rel:
- self
properties:
  name: Access
  sort: 3821
  level: 2
  description: Where access to an API is on the table, and might not be publicly available,
    or part of all plans. Differing from API access as an element, this is about actually
    limiting entire APIs from various groups and plans, and allowing it to be metered
    as part of overall measurements.
entities:
- class:
  - stop
  rel:
  - self
  properties:
    name: Access
  links:
  - rel:
    - self
    href: plans/metrics/access.md
  - rel:
    - parent
    href: plans/metrics/
links:
- rel:
  - self
  href: plans/metrics/access.md
- rel:
  - parent
  href: plans/metrics/
...
