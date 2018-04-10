---
class:
- stop
rel:
- self
properties:
  name: Proxy
  sort: 194
  level: 3
  description: Allowing for the proxying of API requests and responses using tools
    like Charles Proxy, or Prism from Stoplight, and generating of API definitions
    and schemas from the traffic.
  tools:
    - name: Prism
      description: Supercharge any OAS file with mocking, transformations, validations, and more.
      url: https://stoplight.io/platform/prism/
  services:
    - name: Charles
      description: Charles is an HTTP proxy / HTTP monitor / Reverse Proxy that enables a developer to view all of the HTTP and SSL / HTTPS traffic between their machine and the Internet. This includes requests, responses and the HTTP headers (which contain the cookies and caching information).
      url: https://www.charlesproxy.com/          
entities:
- class:
  - stop
  rel:
  - self
  properties:
    name: Proxy
  links:
  - rel:
    - self
    href: definitions/utilities/proxy.md
  - rel:
    - parent
    href: definitions/utilities/
links:
- rel:
  - self
  href: definitions/utilities/proxy.md
- rel:
  - parent
  href: definitions/utilities/
...
