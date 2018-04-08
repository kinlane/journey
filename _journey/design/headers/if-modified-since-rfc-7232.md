---
class:
- stop
rel:
- self
properties:
  name: If-Modified-Since (RFC 7232)
  sort: 515
  level: 3
  description: 'The "If-Modified-Since" header field makes a GET or HEAD request method
    conditional on the selected representation modification date being more recent
    than the date provided in the field-value. Transfer of the selected representation
    data is avoided if that data has not changed. '
entities:
- class:
  - stop
  rel:
  - self
  properties:
    name: If-Modified-Since (RFC 7232)
  links:
  - rel:
    - self
    href: design/headers/if-modified-since-rfc-7232.md
  - rel:
    - parent
    href: design/headers/
links:
- rel:
  - self
  href: design/headers/if-modified-since-rfc-7232.md
- rel:
  - parent
  href: design/headers/
...
