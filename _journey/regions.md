---
class:
  - line
rel:
  - /rels/line
properties:
  name: Regions
  sort: 47
  level: 1
  description: >-
    Which regions does a service operate within, making it available in specific
    regions, and jurisdictions–also which regions is it not allowed to operate
    within.
entities:
  - class:
      - line
    rel:
      - '/rels/line '
    properties:
      - name: Regions
    links:
      - rel:
          - self
        href: /journey/regions/
links:
  - rel:
      - self
    href: /regions/
---
