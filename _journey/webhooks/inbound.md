---
class:
- line
rel:
- self
properties:
  name: Inbound
  sort: 2
  level: 2
  description: Usually webhooks are outward bound, but occasionally they have inbound
    characteristics that should be documented and made available to potential consumers.
entities:
- class:
  - line
  rel:
  - self
  properties:
    name: Inbound
  links:
  - rel:
    - self
    href: webhooks/inbound/
  - rel:
    - parent
    href: webhooks/
links:
- rel:
  - self
  href: webhooks/inbound/
- rel:
  - parent
  href: webhooks/
...
