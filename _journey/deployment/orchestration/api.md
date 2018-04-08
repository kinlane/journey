---
class:
- stop
rel:
- self
properties:
  name: API
  sort: 1514
  level: 2
  description: Ensuring that the orchestration layer possess an API, and can leverage
    external 3rd party APIs as part of the build workflow, making sure that we can
    seamlessly execute every step of the process.
entities:
- class:
  - stop
  rel:
  - self
  properties:
    name: API
  links:
  - rel:
    - self
    href: deployment/orchestration/api.md
  - rel:
    - parent
    href: deployment/orchestration/
links:
- rel:
  - self
  href: deployment/orchestration/api.md
- rel:
  - parent
  href: deployment/orchestration/
...
