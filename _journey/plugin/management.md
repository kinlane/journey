---
class:
- stop
rel:
- self
properties:
  name: Management
  sort: 4
  level: 1
  description: The place where platform users can go to manage the platforms they
    have activated, allowing them to configure the details of how it works, as well
    as remove plugins no longer wanted.
entities:
- class:
  - stop
  rel:
  - self
  properties:
    name: Management
  links:
  - rel:
    - self
    href: plugin/management.md
  - rel:
    - parent
    href: plugin/
links:
- rel:
  - self
  href: plugin/management.md
- rel:
  - parent
  href: plugin/
...
