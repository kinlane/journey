---
class:
- stop
rel:
- self
properties:
  name: Buffer Overflow via Environment Variables
  sort: 2
  level: 2
  description: Avoid this pattern that involves causes a buffer overflow through manipulation
    of environment variables, which once the attacker finds that they can modify an
    environment variable, they may try to overflow associated buffers.
entities:
- class:
  - stop
  rel:
  - self
  properties:
    name: Buffer Overflow via Environment Variables
  links:
  - rel:
    - self
    href: security/abuse-of-functionality/buffer-overflow-via-environment-variables.md
  - rel:
    - parent
    href: security/abuse-of-functionality/
links:
- rel:
  - self
  href: security/abuse-of-functionality/buffer-overflow-via-environment-variables.md
- rel:
  - parent
  href: security/abuse-of-functionality/
...
