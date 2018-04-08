---
class:
- stop
rel:
- self
properties:
  name: Retention
  sort: 1835
  level: 1
  description: Defining how long logs are being stored across all systems relevant
    to a services operation, ensuring that each log entry has a time to live (TTL).
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
    href: logging/retention.md
  - rel:
    - parent
    href: logging/
links:
- rel:
  - self
  href: logging/retention.md
- rel:
  - parent
  href: logging/
...
