---
class:
- stop
rel:
- self
properties:
  name: Position (RFC 3648)
  sort: 123
  level: 2
  description: 'When a new member is added to a collection with a client-maintained
    ordering (for example, with PUT, COPY, or MKCOL), its position in the ordering
    can be set with the new Position header. The Position header allows the client
    to specify that an internal member URI should be first in the collection''s ordering,
    last in the collection''s ordering, immediately before some other internal member
    URI in the collection''s ordering, or immediately after some other internal member
    URI in the collection''s ordering. '
entities:
- class:
  - stop
  rel:
  - self
  properties:
    name: Position (RFC 3648)
  links:
  - rel:
    - self
    href: design/headers/position-rfc-3648.md
  - rel:
    - parent
    href: design/headers/
links:
- rel:
  - self
  href: design/headers/position-rfc-3648.md
- rel:
  - parent
  href: design/headers/
...
