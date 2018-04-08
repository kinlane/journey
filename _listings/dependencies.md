---
class:
  - line
rel:
  - /rels/line
properties:
  name: Dependencies
  sort: 8
  level: 1
  description: >-
    Identifying all backend service, code and infrastructure dependencies
    present for each service.
  start: 6,2
  color: 5ED3D3
  direction: E        
entities:
  - class:
      - line
    rel:
      - '/rels/line '
    properties:
      - name: Dependencies
    links:
      - rel:
          - self
        href: /journey/dependencies/
links:
  - rel:
      - self
    href: /dependencies/
---
