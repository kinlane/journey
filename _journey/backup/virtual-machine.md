---
class:
- stop
rel:
- self
properties:
  name: Virtual Machine
  sort: 3261
  level: 2
  description: Providing services and tooling for backing up virtual machines and
    containers, allowing for easy storage and restore of all compute resources.
entities:
- class:
  - stop
  rel:
  - self
  properties:
    name: Virtual Machine
  links:
  - rel:
    - self
    href: backup/virtual-machine.md
  - rel:
    - parent
    href: backup/
links:
- rel:
  - self
  href: backup/virtual-machine.md
- rel:
  - parent
  href: backup/
...
