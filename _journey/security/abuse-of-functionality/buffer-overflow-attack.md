---
class:
- stop
rel:
- self
properties:
  name: Buffer Overflow Attack
  sort: 1
  level: 2
  description: Avoid overwriting of memory fragments of the process, values of the
    IP (Instruction Pointer), BP (Base Pointer) and other registers which can cause
    exceptions, segmentation faults, and other errors to occur.
entities:
- class:
  - stop
  rel:
  - self
  properties:
    name: Buffer Overflow Attack
  links:
  - rel:
    - self
    href: security/abuse-of-functionality/buffer-overflow-attack.md
  - rel:
    - parent
    href: security/abuse-of-functionality/
links:
- rel:
  - self
  href: security/abuse-of-functionality/buffer-overflow-attack.md
- rel:
  - parent
  href: security/abuse-of-functionality/
...
