---
class:
- stop
rel:
- self
properties:
  name: Lock-down New Writes
  sort: 4314
  level: 2
  description: When will all POST, PUT, and other write capabilities be locked down,
    making it easier to stabilize, sync, and migrate for final shut down.
entities:
- class:
  - stop
  rel:
  - self
  properties:
    name: Lock-down New Writes
  links:
  - rel:
    - self
    href: deprecation/runway/lock-down-new-writes.md
  - rel:
    - parent
    href: deprecation/runway/
links:
- rel:
  - self
  href: deprecation/runway/lock-down-new-writes.md
- rel:
  - parent
  href: deprecation/runway/
...
