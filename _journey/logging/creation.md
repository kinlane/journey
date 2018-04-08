---
class:
- stop
rel:
- self
properties:
  name: Creation
  sort: 1829
  level: 1
  description: Identifying EVERYWHERE logs are created and stored, ensuring that there
    is no single log file left untouched, and not aggregated and evaluated as part
    of the entire lifecycle.
entities:
- class:
  - stop
  rel:
  - self
  properties:
    name: Creation
  links:
  - rel:
    - self
    href: logging/creation.md
  - rel:
    - parent
    href: logging/
links:
- rel:
  - self
  href: logging/creation.md
- rel:
  - parent
  href: logging/
...
