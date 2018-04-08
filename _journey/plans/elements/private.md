---
class:
- stop
rel:
- self
properties:
  name: Private
  sort: 3679
  level: 3
  description: Is this plan a private one, available only to a limited audience? While
    the landing page, or overall portal might be publicly available, the API access
    itself requires approval, or existing account access before you can get more details.
    Private APIs are more common than public APIs, but you should think about the
    pros / cons of keeping things private.
entities:
- class:
  - stop
  rel:
  - self
  properties:
    name: Private
  links:
  - rel:
    - self
    href: plans/elements/private.md
  - rel:
    - parent
    href: plans/elements/
links:
- rel:
  - self
  href: plans/elements/private.md
- rel:
  - parent
  href: plans/elements/
...
