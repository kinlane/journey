---
class:
  - line
rel:
  - /rels/line
properties:
  name: Network
  sort: 57
  level: 1
  description: >-
    Information about networks that are setup, used, and allocated for each
    service governing how it can be accessed and consumed.
entities:
  - class:
      - line
    rel:
      - '/rels/line '
    properties:
      - name: Network
    links:
      - rel:
          - self
        href: /journey/network/
links:
  - rel:
      - self
    href: /network/
---
