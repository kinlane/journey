---
class:
- stop
rel:
- self
properties:
  name: Topic (RFC 8030)
  sort: 165
  level: 2
  description: 'A push message topic is a string carried in a Topic header field.
    A topic is used to correlate push messages sent to the same subscription and does
    not convey any other semantics. '
entities:
- class:
  - stop
  rel:
  - self
  properties:
    name: Topic (RFC 8030)
  links:
  - rel:
    - self
    href: design/headers/topic-rfc-8030.md
  - rel:
    - parent
    href: design/headers/
links:
- rel:
  - self
  href: design/headers/topic-rfc-8030.md
- rel:
  - parent
  href: design/headers/
...
