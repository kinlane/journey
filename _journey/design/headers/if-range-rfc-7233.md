---
class:
- stop
rel:
- self
properties:
  name: If-Range (RFC 7233)
  sort: 519
  level: 3
  description: 'If a client has a partial copy of a representation and wishes to have
    an up-to-date copy of the entire representation, it could use the Range header
    field with a conditional GET (using either or both of If-Unmodified-Since and
    If-Match.) However, if the precondition fails because the representation has been
    modified, the client would then have to make a second request to obtain the entire
    current representation. The "If-Range" header field allows a client to "short-circuit"
    the second request. Informally, its meaning is: if the representation is unchanged,
    send me the part(s) that I am requesting in Range; otherwise, send me the entire
    representation. '
entities:
- class:
  - stop
  rel:
  - self
  properties:
    name: If-Range (RFC 7233)
  links:
  - rel:
    - self
    href: design/headers/if-range-rfc-7233.md
  - rel:
    - parent
    href: design/headers/
links:
- rel:
  - self
  href: design/headers/if-range-rfc-7233.md
- rel:
  - parent
  href: design/headers/
...
