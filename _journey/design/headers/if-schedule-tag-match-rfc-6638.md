---
class:
- stop
rel:
- self
properties:
  name: If-Schedule-Tag-Match (RFC 6638)
  sort: 93
  level: 2
  description: 'The If-Schedule-Tag-Match request header field is used with a method
    to make it conditional. Clients can set this header to the value returned in the
    Schedule-Tag response header, or the CALDAV:schedule-tag property, of a scheduling
    object resource previously retrieved from the server to avoid overwriting "consequential"
    changes to the scheduling object resource. '
entities:
- class:
  - stop
  rel:
  - self
  properties:
    name: If-Schedule-Tag-Match (RFC 6638)
  links:
  - rel:
    - self
    href: design/headers/if-schedule-tag-match-rfc-6638.md
  - rel:
    - parent
    href: design/headers/
links:
- rel:
  - self
  href: design/headers/if-schedule-tag-match-rfc-6638.md
- rel:
  - parent
  href: design/headers/
...
