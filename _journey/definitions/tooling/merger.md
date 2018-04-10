---
class:
- stop
rel:
- self
properties:
  name: Merger
  sort: 173
  level: 3
  description: Tooling or other APIs that provide for the merging of common API definition
    formats, allowing the granularity of what elements get merged, or do not get merged.
    Ideally, this is an API, as well as simple web-based or desktop tooling for API
    providers and consumers.
  tools:
    - name: swagger-combine
      description: Combines multiple Swagger schemas into one dereferenced schema.
      url: https://www.npmjs.com/package/swagger-combine   
    - name: swagger-merger
      description: Merge multiple swagger files into a swagger file, support JSON/YAML.
      url: https://www.npmjs.com/package/swagger-merger     
entities:
- class:
  - stop
  rel:
  - self
  properties:
    name: Merger
  links:
  - rel:
    - self
    href: definitions/tooling/merger.md
  - rel:
    - parent
    href: definitions/tooling/
links:
- rel:
  - self
  href: definitions/tooling/merger.md
- rel:
  - parent
  href: definitions/tooling/
...
