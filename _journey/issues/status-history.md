---
class:
- stop
rel:
- self
properties:
  name: Status History
  sort: 4
  level: 1
  description: Providing a history of status, usually by day, and showing results
    month by month, or week by week, as long as status has been tracked for an API.
entities:
- class:
  - stop
  rel:
  - self
  properties:
    name: Status History
  links:
  - rel:
    - self
    href: issues/status-history.md
  - rel:
    - parent
    href: issues/
links:
- rel:
  - self
  href: issues/status-history.md
- rel:
  - parent
  href: issues/
...
