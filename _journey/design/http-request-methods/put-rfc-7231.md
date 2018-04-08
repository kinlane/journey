---
class:
- stop
rel:
- self
properties:
  name: PUT (RFC 7231)
  sort: 310
  level: 2
  description: 'The PUT method requests that the state of the target resource be created
    or replaced with the state defined by the representation enclosed in the request
    message payload. A successful PUT of a given representation would suggest that
    a subsequent GET on that same target resource will result in an equivalent representation
    being sent in a 200 (OK) response. However, there is no guarantee that such a
    state change will be observable, since the target resource might be acted upon
    by other user agents in parallel, or might be subject to dynamic processing by
    the origin server, before any subsequent GET is received. A successful response
    only implies that the user agent''s intent was achieved at the time of its processing
    by the origin server. '
entities:
- class:
  - stop
  rel:
  - self
  properties:
    name: PUT (RFC 7231)
  links:
  - rel:
    - self
    href: design/http-request-methods/put-rfc-7231.md
  - rel:
    - parent
    href: design/http-request-methods/
links:
- rel:
  - self
  href: design/http-request-methods/put-rfc-7231.md
- rel:
  - parent
  href: design/http-request-methods/
...
