---
class:
- stop
rel:
- self
properties:
  name: On-Demand
  sort: 3693
  level: 3
  description: The resource or set of resources can be deployed, and shut down on
    demand. Each resource can be evaluated for how long it should be available. With
    current approaches to virtualizations, it is easier to make API resources available
    on demand, similar to how Amazon has done with many of their cloud compute resources.
entities:
- class:
  - stop
  rel:
  - self
  properties:
    name: On-Demand
  links:
  - rel:
    - self
    href: plans/elements/on-demand.md
  - rel:
    - parent
    href: plans/elements/
links:
- rel:
  - self
  href: plans/elements/on-demand.md
- rel:
  - parent
  href: plans/elements/
...
