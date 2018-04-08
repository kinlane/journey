---
class:
- line
rel:
- self
properties:
  name: Notification
  sort: 2110
  level: 2
  description: Enabling the ability to send notifications in response to testing activity
    and events as they occur using common channels that key stakeholders will be using.
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
    href: testing/notification/
  - rel:
    - parent
    href: testing/
links:
- rel:
  - self
  href: testing/notification/
- rel:
  - parent
  href: testing/
...
