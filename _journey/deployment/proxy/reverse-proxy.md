---
class:
- stop
rel:
- self
properties:
  name: Reverse Proxy
  sort: 1094
  level: 2
  description: An intermediary for servers to be contacted by any client, allowing
    for transformations and filtering before delivery.
entities:
- class:
  - stop
  rel:
  - self
  properties:
    name: Reverse Proxy
  links:
  - rel:
    - self
    href: deployment/proxy/reverse-proxy.md
  - rel:
    - parent
    href: deployment/proxy/
links:
- rel:
  - self
  href: deployment/proxy/reverse-proxy.md
- rel:
  - parent
  href: deployment/proxy/
...
