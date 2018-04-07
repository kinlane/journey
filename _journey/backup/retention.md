---
class:
- stop
rel:
- self
properties:
  name: Retention
  sort: 5
  level: 1
  description: Determine the constraints, and process for determining and managing
    retention of backups across all services, properly defining how long anything
    should be kept.
entities:
- class:
  - stop
  rel:
  - self
  properties:
    name: Retention
  links:
  - rel:
    - self
    href: backup/retention.md
  - rel:
    - parent
    href: backup/
links:
- rel:
  - self
  href: backup/retention.md
- rel:
  - parent
  href: backup/
...
