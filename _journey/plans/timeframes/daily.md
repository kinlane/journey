---
class:
- stop
rel:
- self
properties:
  name: Daily
  sort: 4
  level: 2
  description: Managing, guiding, and restricting plan entries in days. Like seconds
    and minutes this is a common timeframe for considering rate limits, and judging
    the overall volume requirements of different users. Availability in seconds is
    often directly linked to compute resources being applied as part of operations,
    and tie in with overall availability.
entities:
- class:
  - stop
  rel:
  - self
  properties:
    name: Daily
  links:
  - rel:
    - self
    href: plans/timeframes/daily.md
  - rel:
    - parent
    href: plans/timeframes/
links:
- rel:
  - self
  href: plans/timeframes/daily.md
- rel:
  - parent
  href: plans/timeframes/
...
