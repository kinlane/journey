---
class:
- stop
rel:
- self
properties:
  name: Validator
  sort: 163
  level: 3
  description: Validates an API definition against its formal specification and schema,
    producing a valid or invalid response, with as much detail as possible.
  tools:
    - name: OpenAPI Spec Validator
      description: OpenAPI Spec Validator is a Python library that validates OpenAPI Specs against the OpenAPI 2.0 (aka Swagger) and OpenAPI 3.0.0 specification. The validator aims to check for full compliance with the Specification.
      url: https://github.com/p1c2u/openapi-spec-validator
entities:
- class:
  - stop
  rel:
  - self
  properties:
    name: Validator
  links:
  - rel:
    - self
    href: definitions/tooling/validator.md
  - rel:
    - parent
    href: definitions/tooling/
links:
- rel:
  - self
  href: definitions/tooling/validator.md
- rel:
  - parent
  href: definitions/tooling/
...
