---
class:
- stop
rel:
- self
properties:
  name: Generator
  sort: 159
  level: 3
  description: Generating an API definition format from an existing system or platform,
    outputting the portable machine readable format.
  tools:
    - name: rest-openapi-generator (Node.js)
      description: RESTful Open API Spec generator with resource definitions.
      url: https://www.npmjs.com/package/rest-openapi-generator
    - name: apispec (Python)
      description: A pluggable API specification generator. Currently supports the OpenAPI specification (f.k.a. Swagger 2.0).
      url: https://apispec.readthedocs.io/en/latest/
    - name: swagger-php (PHP)
      description: Generate interactive Swagger documentation for your RESTful API using doctrine annotations.
      url: https://github.com/zircote/swagger-php
    - name: Springfox (Java)
      description: Automated JSON API documentation for API's built with Spring.
      url: http://springfox.github.io/springfox/
    - name: Swagger Core library (Java)
      description: Swagger-core is the Java implementation of Swagger. Current version supports JAX-RS and plain servlets. Integration with the Play! framework has been moved to Swagger-Play.
      url:  https://github.com/swagger-api/swagger-core
    - name: hapi-swagger (Node.js)
      description: This is a OpenAPI (aka Swagger) plug-in for HAPI When installed it will self document the API interface in a project.
      url: https://www.npmjs.com/package/hapi-swagger
    - name: Django REST Swagger (Python)
      description: An API documentation generator for Swagger UI and Django REST Framework
      url: https://github.com/marcgibbons/django-rest-swagger                                     
entities:
- class:
  - stop
  rel:
  - self
  properties:
    name: Generator
  links:
  - rel:
    - self
    href: definitions/tooling/generator.md
  - rel:
    - parent
    href: definitions/tooling/
links:
- rel:
  - self
  href: definitions/tooling/generator.md
- rel:
  - parent
  href: definitions/tooling/
...
