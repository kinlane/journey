---
class:
- stop
rel:
- self
properties:
  name: Converter
  sort: 165
  level: 3
  description: The conversion of an API definition from one format into another, allowing
    designers to share API definitions in any format.
  tools:
    - name: Gnostic
      description: This repository contains a Go command line tool which converts JSON and YAML OpenAPI descriptions to and from equivalent Protocol Buffer representations.
      url:
    - name: swagger2openapi
      description: Convert Swagger 2.0 definitions into OpenApi 3.0.x.
      url: https://github.com/Mermade/swagger2openapi
    - name: OASIS OData
      description: The purpose of this repository is to support development of tools for producing OpenAPI descriptions for OData services.
      url: https://github.com/oasis-tcs/odata-openapi
  services:
    - name: API Transformer
      description: A service with a UI and API for converting API definitions from one format into another, working with many of the popular formats available.
      url: https://apimatic.io/transformer    
entities:
- class:
  - stop
  rel:
  - self
  properties:
    name: Converter
  links:
  - rel:
    - self
    href: definitions/tooling/converter.md
  - rel:
    - parent
    href: definitions/tooling/
links:
- rel:
  - self
  href: definitions/tooling/converter.md
- rel:
  - parent
  href: definitions/tooling/
...
