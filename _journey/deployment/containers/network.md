---
class:
- stop
rel:
- self
properties:
  name: Network
  sort: 1377
  level: 3
  description: Allowing for the configuration of the underlying network for each container
    that is powering different types of services.
entities:
- class:
  - stop
  rel:
  - self
  properties:
    name: Network
  links:
  - rel:
    - self
    href: deployment/containers/network.md
  - rel:
    - parent
    href: deployment/containers/
links:
- rel:
  - self
  href: deployment/containers/network.md
- rel:
  - parent
  href: deployment/containers/
...
