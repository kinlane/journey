---
class:
- stop
rel:
- self
properties:
  name: Offline
  sort: 9
  level: 2
  description: Provide graceful degradation of services when their is no network connection,
    allowing for seamless on and offline transitions.
entities:
- class:
  - stop
  rel:
  - self
  properties:
    name: Offline
  links:
  - rel:
    - self
    href: real-time/features/offline.md
  - rel:
    - parent
    href: real-time/features/
links:
- rel:
  - self
  href: real-time/features/offline.md
- rel:
  - parent
  href: real-time/features/
...
