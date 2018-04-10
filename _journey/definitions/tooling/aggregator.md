---
class:
- stop
rel:
- self
properties:
  name: Aggregator
  sort: 169
  level: 3
  description: Aggregation of APIs using a machine readable API definition format, allowing multiple APIs to be aggregated into a single definition, either combining or merging using API definitions.
  tools:
    - name: swagger-aggregator
      description: Swagger-aggregator allow you to create a swagger REST API from several other swagger REST APIs. This can be really useful if you want to make an API Gateway accessing some of your internal APIs. You can also filter which path you want to deliver, and which properties of your definitions you don't want to show.
      url: https://github.com/Trax-air/swagger-aggregator
entities:
- class:
  - stop
  rel:
  - self
  properties:
    name: Aggregator
  links:
  - rel:
    - self
    href: definitions/tooling/aggregator.md
  - rel:
    - parent
    href: definitions/tooling/
links:
- rel:
  - self
  href: definitions/tooling/aggregator.md
- rel:
  - parent
  href: definitions/tooling/
...
