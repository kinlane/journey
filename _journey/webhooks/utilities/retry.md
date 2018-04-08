---
class:
- stop
rel:
- self
properties:
  name: Retry
  sort: 3
  level: 2
  description: Allowing for the retry of any webhook, based upon specific events or
    schedule.
entities:
- class:
  - stop
  rel:
  - self
  properties:
    name: Retry
  links:
  - rel:
    - self
    href: webhooks/utilities/retry.md
  - rel:
    - parent
    href: webhooks/utilities/
links:
- rel:
  - self
  href: webhooks/utilities/retry.md
- rel:
  - parent
  href: webhooks/utilities/
...
