---
class:
- stop
rel:
- self
properties:
  name: Email
  sort: 2
  level: 2
  description: Provide notifications about DNS layer via emails.
entities:
- class:
  - stop
  rel:
  - self
  properties:
    name: Email
  links:
  - rel:
    - self
    href: dns/notifications/email.md
  - rel:
    - parent
    href: dns/notifications/
links:
- rel:
  - self
  href: dns/notifications/email.md
- rel:
  - parent
  href: dns/notifications/
...
