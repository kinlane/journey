---
class:
- stop
rel:
- self
properties:
  name: Event
  sort: 3
  level: 2
  description: Selecting which events triggers a Webhook.
entities:
- class:
  - stop
  rel:
  - self
  properties:
    name: Event
  links:
  - rel:
    - self
    href: webhooks/core/event.md
  - rel:
    - parent
    href: webhooks/core/
links:
- rel:
  - self
  href: webhooks/core/event.md
- rel:
  - parent
  href: webhooks/core/
...
