---
class:
- stop
rel:
- self
properties:
  name: Target Endpoint
  sort: 1106
  level: 2
  description: The URL of the target being proxied, allowing for the backend connection
    of existing resources, and the delivered via proxy.
entities:
- class:
  - stop
  rel:
  - self
  properties:
    name: Target Endpoint
  links:
  - rel:
    - self
    href: deployment/proxy/target-endpoint.md
  - rel:
    - parent
    href: deployment/proxy/
links:
- rel:
  - self
  href: deployment/proxy/target-endpoint.md
- rel:
  - parent
  href: deployment/proxy/
...
