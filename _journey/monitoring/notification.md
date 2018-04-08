---
class:
- line
rel:
- self
properties:
  name: Notification
  sort: 5
  level: 2
  description: Enabling the ability to send notifications in response to monitoring
    activity and events as they occur using common channels that key stakeholders
    will be using.
entities:
- class:
  - line
  rel:
  - self
  properties:
    name: Notification
  links:
  - rel:
    - self
    href: monitoring/notification/
  - rel:
    - parent
    href: monitoring/
links:
- rel:
  - self
  href: monitoring/notification/
- rel:
  - parent
  href: monitoring/
...
