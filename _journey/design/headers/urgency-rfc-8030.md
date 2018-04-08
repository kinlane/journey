---
class:
- stop
rel:
- self
properties:
  name: Urgency (RFC 8030)
  sort: 677
  level: 3
  description: 'An application server MAY include an Urgency header field in its request
    for push message delivery. This header field indicates the message urgency. The
    push service MUST NOT forward the Urgency header field to the user agent. A push
    message without the Urgency header field defaults to a value of "normal". '
entities:
- class:
  - stop
  rel:
  - self
  properties:
    name: Urgency (RFC 8030)
  links:
  - rel:
    - self
    href: design/headers/urgency-rfc-8030.md
  - rel:
    - parent
    href: design/headers/
links:
- rel:
  - self
  href: design/headers/urgency-rfc-8030.md
- rel:
  - parent
  href: design/headers/
...
