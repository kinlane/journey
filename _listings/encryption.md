---
class:
  - line
rel:
  - /rels/line
properties:
  name: Encryption
  sort: 21
  level: 1
  description: >-
    Details regarding what is expected regarding encryption on disk, as well as
    in transport for each service.
  start: 4
  color: 2B4F3C
  direction: N     
entities:
  - class:
      - line
    rel:
      - '/rels/line '
    properties:
      - name: Encryption
    links:
      - rel:
          - self
        href: /journey/encryption/
links:
  - rel:
      - self
    href: /encryption/
---
