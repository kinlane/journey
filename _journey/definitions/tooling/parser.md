---
class:
- stop
rel:
- self
properties:
  name: Parser
  sort: 161
  level: 3
  description: Parses a machine readable API definition and makes ready for use in specific language, structure, or platform.
  tools:
    - name: KaiZen OpenAPI Parser
      description: The KaiZen OpenApi Parser from RepreZen is a Java-based validating parser for OpenAPI 3.0 offering full compliance with the OpenAPI 3.0 Specification, and a highly uniform read/write programming API. OpenAPI, formerly known as the Swagger specification, is the industry-standard format for machine-readable REST API descriptions.
      url: https://github.com/RepreZen/KaiZen-OpenApi-Parser
    - name: PSX
      description: PSX provides tools to handle common API tasks like data serialization, validation, documentation, API versioning and testing. So you can concentrate on building the actual business logic of your API.
      url: http://phpsx.org/
    - name: OpenAPI 3 Parser
      description: This is a parser/validator for Open API 3 built in Ruby.
      url: https://github.com/kevindew/openapi3_parser   
entities:
- class:
  - stop
  rel:
  - self
  properties:
    name: Parser
  links:
  - rel:
    - self
    href: definitions/tooling/parser.md
  - rel:
    - parent
    href: definitions/tooling/
links:
- rel:
  - self
  href: definitions/tooling/parser.md
- rel:
  - parent
  href: definitions/tooling/
...
