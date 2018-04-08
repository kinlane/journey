---
class:
- stop
rel:
- self
properties:
  name: Commands
  sort: 2
  level: 1
  description: Providing a list of the available commands that can be applied to commands
    and put services to work on the platform.
entities:
- class:
  - stop
  rel:
  - self
  properties:
    name: Commands
  links:
  - rel:
    - self
    href: command-line-interface/commands.md
  - rel:
    - parent
    href: command-line-interface/
links:
- rel:
  - self
  href: command-line-interface/commands.md
- rel:
  - parent
  href: command-line-interface/
...
