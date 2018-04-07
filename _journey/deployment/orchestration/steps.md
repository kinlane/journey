---
class:
- stop
rel:
- self
properties:
  name: Steps
  sort: 5
  level: 2
  description: Precise modeling of each step in the deployment of each service, providing
    everything that is needed from start to finish.
entities:
- class:
  - stop
  rel:
  - self
  properties:
    name: Steps
  links:
  - rel:
    - self
    href: deployment/orchestration/steps.md
  - rel:
    - parent
    href: deployment/orchestration/
links:
- rel:
  - self
  href: deployment/orchestration/steps.md
- rel:
  - parent
  href: deployment/orchestration/
...
