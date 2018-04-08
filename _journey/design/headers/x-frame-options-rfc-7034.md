---
class:
- stop
rel:
- self
properties:
  name: X-Frame-Options (RFC 7034)
  sort: 699
  level: 3
  description: 'The X-Frame-Options HTTP header field indicates a policy that specifies
    whether the browser should render the transmitted resource within a or an . Servers
    can declare this policy in the header of their HTTP responses to prevent clickjacking
    attacks, which ensures that their content is not embedded into other pages or
    frames. '
entities:
- class:
  - stop
  rel:
  - self
  properties:
    name: X-Frame-Options (RFC 7034)
  links:
  - rel:
    - self
    href: design/headers/x-frame-options-rfc-7034.md
  - rel:
    - parent
    href: design/headers/
links:
- rel:
  - self
  href: design/headers/x-frame-options-rfc-7034.md
- rel:
  - parent
  href: design/headers/
...
