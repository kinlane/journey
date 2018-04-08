---
class:
- stop
rel:
- self
properties:
  name: Infrequent
  sort: 3703
  level: 3
  description: Resources are accessed infrequently, treating them as warehoused, or
    off to the side. Another side of the resource availability which focuses on these
    infrequent levels of access, and may allow a users access or plan shift from infrequent,
    to higher levels, if rate limits are exceeded.
entities:
- class:
  - stop
  rel:
  - self
  properties:
    name: Infrequent
  links:
  - rel:
    - self
    href: plans/elements/infrequent.md
  - rel:
    - parent
    href: plans/elements/
links:
- rel:
  - self
  href: plans/elements/infrequent.md
- rel:
  - parent
  href: plans/elements/
...
