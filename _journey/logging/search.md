---
class:
- stop
rel:
- self
properties:
  name: Search
  sort: 12
  level: 1
  description: Allowing for each search across all aggregated log files, looking by
    keyword, tags, source, application, and other relevant data points that will matter
    to operations.
entities:
- class:
  - stop
  rel:
  - self
  properties:
    name: Search
  links:
  - rel:
    - self
    href: logging/search.md
  - rel:
    - parent
    href: logging/
links:
- rel:
  - self
  href: logging/search.md
- rel:
  - parent
  href: logging/
...
