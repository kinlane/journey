---
class:
- stop
rel:
- self
properties:
  name: Action
  sort: 4
  level: 2
  description: Allow for standard actions to be taken across resource, but also reflect
    how APIs will be experienced, providing meaningful action to be taken around any
    API.
entities:
- class:
  - stop
  rel:
  - self
  properties:
    name: Action
  links:
  - rel:
    - self
    href: design/http-requests/action.md
  - rel:
    - parent
    href: design/http-requests/
links:
- rel:
  - self
  href: design/http-requests/action.md
- rel:
  - parent
  href: design/http-requests/
...
