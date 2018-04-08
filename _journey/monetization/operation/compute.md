---
class:
- stop
rel:
- self
properties:
  name: Compute
  sort: 2
  level: 2
  description: What percentage of my AWS compute is dedicated to an API. Flat percentage
    of the server its one until usage history exists.
entities:
- class:
  - stop
  rel:
  - self
  properties:
    name: Compute
  links:
  - rel:
    - self
    href: monetization/operation/compute.md
  - rel:
    - parent
    href: monetization/operation/
links:
- rel:
  - self
  href: monetization/operation/compute.md
- rel:
  - parent
  href: monetization/operation/
...
