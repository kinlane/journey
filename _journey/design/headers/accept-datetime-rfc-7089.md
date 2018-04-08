---
class:
- stop
rel:
- self
properties:
  name: Accept-Datetime (RFC 7089)
  sort: 351
  level: 3
  description: 'The "Accept-Datetime" request header is transmitted by a user agent
    to indicate it wants to access a past state of an Original Resource. To that end,
    the "Accept-Datetime" header is conveyed in an HTTP request issued against a TimeGate
    for an Original Resource, and its value indicates the datetime of the desired
    past state of the Original Resource. '
entities:
- class:
  - stop
  rel:
  - self
  properties:
    name: Accept-Datetime (RFC 7089)
  links:
  - rel:
    - self
    href: design/headers/accept-datetime-rfc-7089.md
  - rel:
    - parent
    href: design/headers/
links:
- rel:
  - self
  href: design/headers/accept-datetime-rfc-7089.md
- rel:
  - parent
  href: design/headers/
...
