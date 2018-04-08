---
class:
- stop
rel:
- self
properties:
  name: Tests
  sort: 1500
  level: 2
  description: Building in tests for the entire servicestack into the orchestration
    environment, ensuring consistent and reliable deployment of services.
entities:
- class:
  - stop
  rel:
  - self
  properties:
    name: Tests
  links:
  - rel:
    - self
    href: deployment/orchestration/tests.md
  - rel:
    - parent
    href: deployment/orchestration/
links:
- rel:
  - self
  href: deployment/orchestration/tests.md
- rel:
  - parent
  href: deployment/orchestration/
...
