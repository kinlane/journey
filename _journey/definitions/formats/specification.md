---
class:
- stop
rel:
- self
properties:
  name: Specification
  sort: 148
  level: 3
  description: The root specification for the API definition format, providing a base
    set of rules for all services and tools that employ the spec.
  tools:
    - name: OpenAPI
      description: The OpenAPI Initiative (OAI) was created by a consortium of forward-looking industry experts who recognize the immense value of standardizing on how REST APIs are described. As an open governance structure under the Linux Foundation, the OAI is focused on creating, evolving and promoting a vendor neutral description format. SmartBear Software is donating the Swagger Specification directly to the OAI as the basis of this Open Specification.
      url: https://www.openapis.org/
    - name: API Blueprint
      description: API Blueprint is simple and accessible to everybody involved in the API lifecycle. Its syntax is concise yet expressive. With API Blueprint you can quickly design and prototype APIs to be created or document and test already deployed mission-critical APIs.
      url: https://apiblueprint.org/   
    - name: RAML
      description: RESTful API Modeling Language (RAML) makes it easy to manage the whole API lifecycle from design to sharing. It's concise - you only write what you need to define - and reusable. It is machine readable API design that is actually human friendly.
      url: https://raml.org/     
    - name: Postman Collection
      description: A Postman Collection is an executable API description. Postman is an app for making HTTP requests, and Postman collections help you organize and group related API requests. Collections can make custom connector development faster and easier if you don't already have an OpenAPI definition for your API.
      url: https://apiblueprint.org/                     
entities:
- class:
  - stop
  rel:
  - self
  properties:
    name: Specification
  links:
  - rel:
    - self
    href: definitions/formats/specification.md
  - rel:
    - parent
    href: definitions/formats/
links:
- rel:
  - self
  href: definitions/formats/specification.md
- rel:
  - parent
  href: definitions/formats/
...
