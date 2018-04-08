---
class:
- stop
rel:
- self
properties:
  name: Depth (RFC 4918)
  sort: 69
  level: 2
  description: 'The Depth request header is used with methods executed on resources
    that could potentially have internal members to indicate whether the method is
    to be applied only to the resource ("Depth: 0"), to the resource and its internal
    members only ("Depth: 1"), or the resource and all its members ("Depth: infinity"). '
entities:
- class:
  - stop
  rel:
  - self
  properties:
    name: Depth (RFC 4918)
  links:
  - rel:
    - self
    href: design/headers/depth-rfc-4918.md
  - rel:
    - parent
    href: design/headers/
links:
- rel:
  - self
  href: design/headers/depth-rfc-4918.md
- rel:
  - parent
  href: design/headers/
...
