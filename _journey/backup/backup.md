---
class:
  - line
rel:
  - /rels/line
properties:
  name: Backup
  sort: 53
  level: 1
  description: >-
    What types of backups are in place to bring redundancy to the database,
    server, storage, and other essential aspects of a service’s operations?
entities:
  - class:
      - line
    rel:
      - '/rels/line '
    properties:
      - name: Backup
    links:
      - rel:
          - self
        href: /journey/backup/
links:
  - rel:
      - self
    href: /backup/
---
