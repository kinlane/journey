---
class:
- stop
rel:
- self
properties:
  name: Schema
  sort: 150
  level: 3
  description: A representation of data model, used as part of an API request, or
    response, usually in JSON, but increasingly YAML, and Markdown are also used.
  tools:
    - name: JSON Schema
      description: Describes your JSON data format in clear, human- and machine-readable documentation that is complete structural validation, useful for automated testing, and validating client-submitted data.
      url: http://json-schema.org/
    - name: Application-Level Profile Semantics (ALPS)
      description: The purpose of Application-Level Profile Semantics (ALPS) is to document the application-level semantics of a particular implementation. This is accomplished by describing elements of response representations for a target media type. For example identifying markup elements returned (i.e. semantic HTML ala Microformats) and state transitions (i.e. HTML.A and HTML.FORM elements) that advance the state of the current application.
      url: http://amundsen.com/hypermedia/profiles/
    - name: Schema.org
      description: Schema.org is a collaborative, community activity with a mission to create, maintain, and promote schemas for structured data on the Internet, on web pages, in email messages, and beyond. Schema.org vocabulary can be used with many different encodings, including RDFa, Microdata and JSON-LD.
      url: http://schema.org/                    
entities:
- class:
  - stop
  rel:
  - self
  properties:
    name: Schema
  links:
  - rel:
    - self
    href: definitions/formats/schema.md
  - rel:
    - parent
    href: definitions/formats/
links:
- rel:
  - self
  href: definitions/formats/schema.md
- rel:
  - parent
  href: definitions/formats/
...
