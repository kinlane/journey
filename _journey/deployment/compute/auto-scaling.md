---
class:
- stop
rel:
- self
properties:
  name: Auto Scaling
  sort: 1339
  level: 3
  description: Setting the stage for auto scaling of compute resources will occur,
    allowing the autoscaling of underlying compute for all services.
entities:
- class:
  - stop
  rel:
  - self
  properties:
    name: Auto Scaling
  links:
  - rel:
    - self
    href: deployment/compute/auto-scaling.md
  - rel:
    - parent
    href: deployment/compute/
links:
- rel:
  - self
  href: deployment/compute/auto-scaling.md
- rel:
  - parent
  href: deployment/compute/
...
