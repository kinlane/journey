---
class:
- line
rel:
- self
properties:
  name: Resources
  sort: 8
  level: 2
  description: What other resources are available for use as variables within plans,
    to help refine and incentivize how service usage and consumption occurs beyond
    the usual data points?
entities:
- class:
  - line
  rel:
  - self
  properties:
    name: Resources
  links:
  - rel:
    - self
    href: plans/resources/
  - rel:
    - parent
    href: plans/
links:
- rel:
  - self
  href: plans/resources/
- rel:
  - parent
  href: plans/
...
