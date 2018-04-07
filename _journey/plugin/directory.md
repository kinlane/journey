---
class:
- stop
rel:
- self
properties:
  name: Directory
  sort: 3
  level: 1
  description: The location where all plugins are published for private or public
    consumption, allowing platform users to find new plugins, and turn on as part
    of their platform usage.
entities:
- class:
  - stop
  rel:
  - self
  properties:
    name: Directory
  links:
  - rel:
    - self
    href: plugin/directory.md
  - rel:
    - parent
    href: plugin/
links:
- rel:
  - self
  href: plugin/directory.md
- rel:
  - parent
  href: plugin/
...
