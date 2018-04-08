---
class:
- stop
rel:
- self
properties:
  name: Accept-Post (W3C TR http://www.w3.org/TR/ldp)
  sort: 363
  level: 2
  description: 'The Accept-Post HTTP header SHOULD appear in the OPTIONS response
    for any resource that supports the use of the POST method. The presence of the
    Accept-Post header in response to any method is an implicit indication that POST
    is allowed on the resource identified by the Request-URI. The presence of a specific
    document format in this header indicates that that specific format is allowed
    on POST requests to the resource identified by the Request-URI. '
entities:
- class:
  - stop
  rel:
  - self
  properties:
    name: Accept-Post (W3C TR http://www.w3.org/TR/ldp)
  links:
  - rel:
    - self
    href: design/headers/accept-post-w3c-tr-http-www.w3.org-tr-ldp.md
  - rel:
    - parent
    href: design/headers/
links:
- rel:
  - self
  href: design/headers/accept-post-w3c-tr-http-www.w3.org-tr-ldp.md
- rel:
  - parent
  href: design/headers/
...
