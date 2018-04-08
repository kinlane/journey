---
class:
- stop
rel:
- self
properties:
  name: Archive
  sort: 3705
  level: 3
  description: Resources are in an archived state and require very little access,
    and can be stored in different manner. Like infrequent, archive is mean for maybe
    one-time access, in future dates. Think of these levels as minimum rate limits,
    which base pricing not on volume, but only is cheap if minimum thresholds are
    met.
entities:
- class:
  - stop
  rel:
  - self
  properties:
    name: Archive
  links:
  - rel:
    - self
    href: plans/elements/archive.md
  - rel:
    - parent
    href: plans/elements/
links:
- rel:
  - self
  href: plans/elements/archive.md
- rel:
  - parent
  href: plans/elements/
...
