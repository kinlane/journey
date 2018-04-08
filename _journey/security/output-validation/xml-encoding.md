---
class:
- stop
rel:
- self
properties:
  name: XML Encoding
  sort: 3
  level: 2
  description: Do not assemble XML string concatenation, rather us a XML serializer,
    ensure that the XML content sent to the browser is parseable and does not contain
    XML injection.
entities:
- class:
  - stop
  rel:
  - self
  properties:
    name: XML Encoding
  links:
  - rel:
    - self
    href: security/output-validation/xml-encoding.md
  - rel:
    - parent
    href: security/output-validation/
links:
- rel:
  - self
  href: security/output-validation/xml-encoding.md
- rel:
  - parent
  href: security/output-validation/
...
