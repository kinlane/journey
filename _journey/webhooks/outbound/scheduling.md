---
class:
- stop
rel:
- self
properties:
  name: Scheduling
  sort: 3213
  level: 3
  description: Running code that can be used as webhook target, also as schedule jobs
    allowing them to trigger on schedule instead of just events.
entities:
- class:
  - stop
  rel:
  - self
  properties:
    name: Scheduling
  links:
  - rel:
    - self
    href: webhooks/outbound/scheduling.md
  - rel:
    - parent
    href: webhooks/outbound/
links:
- rel:
  - self
  href: webhooks/outbound/scheduling.md
- rel:
  - parent
  href: webhooks/outbound/
...
