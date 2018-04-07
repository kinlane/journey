---
class:
  - line
rel:
  - /rels/line
properties:
  name: Client
  sort: 30
  level: 1
  description: >-
    Information about clients being used to interface with and work with the
    service, allowing it to be put to use without code.
entities:
  - class:
      - line
    rel:
      - '/rels/line '
    properties:
      - name: Client
    links:
      - rel:
          - self
        href: /journey/client/
links:
  - rel:
      - self
    href: /client/
---
