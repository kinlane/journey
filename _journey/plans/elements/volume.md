---
class:
- stop
rel:
- self
properties:
  name: Volume
  sort: 10
  level: 2
  description: Volume pricing levels are available, with plans based entirely on volume
    level access to resources. Some platforms operate entirely on volume levels of
    API access, and levels should be crafted with end consumers in mind, and how they
    will be consumed, and at what levels.
entities:
- class:
  - stop
  rel:
  - self
  properties:
    name: Volume
  links:
  - rel:
    - self
    href: plans/elements/volume.md
  - rel:
    - parent
    href: plans/elements/
links:
- rel:
  - self
  href: plans/elements/volume.md
- rel:
  - parent
  href: plans/elements/
...
