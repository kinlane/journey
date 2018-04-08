---
class:
  - line
rel:
  - /rels/line
properties:
  name: Aggregation
  sort: 42
  level: 1
  description: >-
    Are there any aggregation solutions in place that involve the service, and
    depend on its availability?
  x: 0
  y: 2
  color: DE3511
  direction: S
entities:
  - class:
      - line
    rel:
      - '/rels/line '
    properties:
      - name: Aggregation
    links:
      - rel:
          - self
        href: /journey/aggregation/
links:
  - rel:
      - self
    href: /aggregation/
---
