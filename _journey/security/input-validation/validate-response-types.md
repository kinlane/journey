---
class:
- stop
rel:
- self
properties:
  name: Validate Response Types
  sort: 2379
  level: 2
  description: Do NOT simply copy the Accept header to the Content-type header of
    the response, and reject the request if the Accept header does not specifically
    contain one of the allowable types.
entities:
- class:
  - stop
  rel:
  - self
  properties:
    name: Validate Response Types
  links:
  - rel:
    - self
    href: security/input-validation/validate-response-types.md
  - rel:
    - parent
    href: security/input-validation/
links:
- rel:
  - self
  href: security/input-validation/validate-response-types.md
- rel:
  - parent
  href: security/input-validation/
...
