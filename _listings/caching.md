---
class:
  - line
rel:
  - /rels/line
properties:
  name: Caching
  sort: 3
  level: 1
  description: >-
    What caching exists at the server, CDN, and DNS layers for each service to
    provide a higher level of performance?
  x: 0
  y: 14
  color: C28FDE
  direction: S      
entities:
  - class:
      - line
    rel:
      - '/rels/line '
    properties:
      - name: Caching
    links:
      - rel:
          - self
        href: /journey/caching/
links:
  - rel:
      - self
    href: /caching/
---
