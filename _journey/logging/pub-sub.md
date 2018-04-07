---
class:
- stop
rel:
- self
properties:
  name: Pub/Sub
  sort: 10
  level: 1
  description: Providing a publish / subscribe platform using Websub that identifying
    logging topics, and establishes channels that relevant users, systems, and applications
    can subscribe to the channels they need.
entities:
- class:
  - stop
  rel:
  - self
  properties:
    name: Pub/Sub
  links:
  - rel:
    - self
    href: logging/pub-sub.md
  - rel:
    - parent
    href: logging/
links:
- rel:
  - self
  href: logging/pub-sub.md
- rel:
  - parent
  href: logging/
...
