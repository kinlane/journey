---
class:
- stop
rel:
- self
properties:
  name: Used Regions
  sort: 3
  level: 1
  description: A real time, working list of regions that are in use as part of platform
    operations, showing where services are deployed permanently or temporarily.
entities:
- class:
  - stop
  rel:
  - self
  properties:
    name: Used Regions
  links:
  - rel:
    - self
    href: regions/used-regions.md
  - rel:
    - parent
    href: regions/
links:
- rel:
  - self
  href: regions/used-regions.md
- rel:
  - parent
  href: regions/
...
