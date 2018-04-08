---
class:
- stop
rel:
- self
properties:
  name: Schedule-Reply (RFC 6638)
  sort: 607
  level: 3
  description: 'The Schedule-Reply request header is used by a client to indicate
    to a server whether or not a scheduling operation ought to occur when an "Attendee"
    deletes a scheduling object resource. In particular, it controls whether a reply
    scheduling message is sent to the "Organizer" as a result of the removal. There
    are situations in which unsolicited scheduling messages need to be silently removed
    (or ignored) for security or privacy reasons. This request header allows the scheduling
    object resource to be removed if such a need arises. '
entities:
- class:
  - stop
  rel:
  - self
  properties:
    name: Schedule-Reply (RFC 6638)
  links:
  - rel:
    - self
    href: design/headers/schedule-reply-rfc-6638.md
  - rel:
    - parent
    href: design/headers/
links:
- rel:
  - self
  href: design/headers/schedule-reply-rfc-6638.md
- rel:
  - parent
  href: design/headers/
...
