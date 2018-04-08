---
class:
- stop
rel:
- self
properties:
  name: Dedicated
  sort: 3701
  level: 3
  description: Resources can be allocated in a dedicated state, remaining available
    with no downtime, or according to SLA. This element is complementary to on-demand,
    and reserved instances, where the resources can be purchased on a dedicated bases.
    For many API resources dedicated will be the default state, and not worth mentioning
    unless on-demand, and other elements are available.
entities:
- class:
  - stop
  rel:
  - self
  properties:
    name: Dedicated
  links:
  - rel:
    - self
    href: plans/elements/dedicated.md
  - rel:
    - parent
    href: plans/elements/
links:
- rel:
  - self
  href: plans/elements/dedicated.md
- rel:
  - parent
  href: plans/elements/
...
