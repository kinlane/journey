---
class:
- line
rel:
- self
properties:
  name: DNS
  sort: 1215
  level: 3
  description: Allowing for the management of DNS associated with scraping, allowing
    for domains to be efficiently targeted, and excluded depending on what is needed.
entities:
- class:
  - line
  rel:
  - self
  properties:
    name: DNS
  links:
  - rel:
    - self
    href: deployment/scraping/dns/
  - rel:
    - parent
    href: deployment/scraping/
links:
- rel:
  - self
  href: deployment/scraping/dns/
- rel:
  - parent
  href: deployment/scraping/
...
