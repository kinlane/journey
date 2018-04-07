---
class:
- stop
rel:
- self
properties:
  name: Presence
  sort: 1
  level: 2
  description: Presence provides information on when a user has joined or left a channel,
    who, and how many, users are subscribed to a particular channel, which channel(s)
    an individual user is subscribed to associated state information for these users,
    which may include latitude / longitude, typing status, and more.
entities:
- class:
  - stop
  rel:
  - self
  properties:
    name: Presence
  links:
  - rel:
    - self
    href: real-time/features/presence.md
  - rel:
    - parent
    href: real-time/features/
links:
- rel:
  - self
  href: real-time/features/presence.md
- rel:
  - parent
  href: real-time/features/
...
