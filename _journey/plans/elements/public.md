---
class:
- stop
rel:
- self
properties:
  name: Public
  sort: 2
  level: 2
  description: Is this a publicly available API operation, something that may only
    apply to some plans? While not all aspects of API operations will be 100% publicly
    available, there are some elements that anyone from the public can gain access
    to, even if it is rate limited in some way.
entities:
- class:
  - stop
  rel:
  - self
  properties:
    name: Public
  links:
  - rel:
    - self
    href: plans/elements/public.md
  - rel:
    - parent
    href: plans/elements/
links:
- rel:
  - self
  href: plans/elements/public.md
- rel:
  - parent
  href: plans/elements/
...
