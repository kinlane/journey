---
class:
  - line
rel:
  - /rels/line
properties:
  name: DNS
  sort: 8
  level: 1
  description: >-
    The domain addressing being used for routing, management and auditing of all
    service traffic, opening up this layer of the stack to be accessible as part
    of the API lifecycle.
  x: 16
  y: 0
  color: FD0826
  direction: E     
entities:
  - class:
      - line
    rel:
      - '/rels/line '
    properties:
      - name: DNS
    links:
      - rel:
          - self
        href: /journey/dns/
links:
  - rel:
      - self
    href: /dns/
---
