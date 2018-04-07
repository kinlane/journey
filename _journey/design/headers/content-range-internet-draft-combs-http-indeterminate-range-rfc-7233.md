---
class:
- stop
rel:
- self
properties:
  name: Content-Range (Internet Draft combs-http-indeterminate-range RFC 7233)
  sort: 52
  level: 2
  description: 'The Content-Range entity-header is sent with a partial entity-body
    to specify where in the full entity-body the partial body should be applied.The
    "Content-Range" header field is sent in a single part 206 (Partial Content) response
    to indicate the partial range of the selected representation enclosed as the message
    payload, sent in each part of a multipart 206 response to indicate the range enclosed
    within each body part, and sent in 416 (Range Not Satisfiable) responses to provide
    information about the selected representation. '
entities:
- class:
  - stop
  rel:
  - self
  properties:
    name: Content-Range (Internet Draft combs-http-indeterminate-range RFC 7233)
  links:
  - rel:
    - self
    href: design/headers/content-range-internet-draft-combs-http-indeterminate-range-rfc-7233.md
  - rel:
    - parent
    href: design/headers/
links:
- rel:
  - self
  href: design/headers/content-range-internet-draft-combs-http-indeterminate-range-rfc-7233.md
- rel:
  - parent
  href: design/headers/
...
