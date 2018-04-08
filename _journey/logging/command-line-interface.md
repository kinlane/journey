---
class:
- stop
rel:
- self
properties:
  name: Command Line Interface
  sort: 13
  level: 1
  description: Enable a command line interface at the aggregate log level, allowing
    for easy programmatic integration, orchestration, and integrated into the larger
    continuous build process.
entities:
- class:
  - stop
  rel:
  - self
  properties:
    name: Command Line Interface
  links:
  - rel:
    - self
    href: logging/command-line-interface.md
  - rel:
    - parent
    href: logging/
links:
- rel:
  - self
  href: logging/command-line-interface.md
- rel:
  - parent
  href: logging/
...