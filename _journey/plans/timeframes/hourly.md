---
class:
- stop
rel:
- self
properties:
  name: Hourly
  sort: 3
  level: 2
  description: Managing, guiding, and restricting plan entries in hours. While there
    may be rate limits at the hourly level, this timeframe is more applied to resources
    that are on-demand and ephemeral, and can be consumed as needed, in a utility
    style that is becoming common way to plan API access.
entities:
- class:
  - stop
  rel:
  - self
  properties:
    name: Hourly
  links:
  - rel:
    - self
    href: plans/timeframes/hourly.md
  - rel:
    - parent
    href: plans/timeframes/
links:
- rel:
  - self
  href: plans/timeframes/hourly.md
- rel:
  - parent
  href: plans/timeframes/
...
