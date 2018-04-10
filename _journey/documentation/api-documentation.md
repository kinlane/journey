---
class:
- line
rel:
- self
properties:
  name: API Documentation
  sort: 1689
  level: 2
  description: The details of an API's surface area, with all the details needed to
    put to services work, and be able to full integrate with the platform.
  tools:
    - name: Swagger UI
      description: Swagger UI allows anyone — be it your development team or your end consumers — to visualize and interact with the API’s resources without having any of the implementation logic in place. It’s automatically generated from your Swagger specification, with the visual documentation making it easy for back end implementation and client side consumption.
      url: https://swagger.io/swagger-ui/
    - name: ReDoc
      description: OpenAPI/Swagger-generated API Reference Documentation.
      url: https://github.com/Rebilly/ReDoc
    - name: DapperDox
      description: DapperDox is Open-Source, and provides rich, out-of-the-box, rendering of your OpenAPI specifications, seamlessly combined with your GitHub Flavored Markdown documentation, guides and diagrams.
      url: http://dapperdox.io/    
  services:
    - name: ReadMe.io
      description: eadMe is a developer hub for your startup or code. It's a completely customizable and collaborative place for documentation, support, key generation and more. Don't waste your precious time reimplementing a dev.yourstartup.com. If you have an API, code library, or affiliate program, documentation is hard. Users can't use your product without understanding it, and most documentation on the Internet is lacking. The goal of ReadMe is to make consuming APIs completely painless.
      url: https://readme.io/
    - name: https://api-docs.io/
      description: Hosted public API documentation for every OAS (Swagger) and RAML specs provided by Stoplight.io.
      url: https://api-docs.io/  
entities:
- class:
  - line
  rel:
  - self
  properties:
    name: API Documentation
  links:
  - rel:
    - self
    href: documentation/api-documentation/
  - rel:
    - parent
    href: documentation/
links:
- rel:
  - self
  href: documentation/api-documentation/
- rel:
  - parent
  href: documentation/
...
