---
class:
- line
rel:
- self
properties:
  name: Proxy
  sort: 1091
  level: 2
  description: A lightweight, service or tool-based approach to getting in the way
    of an existing service and applying transformations on it before the results are
    accessed via consistent services delivered using APIs.
  services:
    - name: Postman Proxy
      description: A proxy server acts as a security barrier between your internal network and the Internet, keeping others on the Internet from accessing information on your internal network.
      url: https://www.getpostman.com/docs/v6/postman/sending_api_requests/proxy   
  tools:
    - name: node-api-proxy
      description: A reverse proxy designed for use with rate limited APIs.
      url: https://github.com/mwilliamson/http-api-proxy
    - name: Node API Proxy
      description: This repository contains everything to run a simpler API proxy. You can either use the deploy button to create everything automatically. It should work in most cases. Or you can clone the repo and do it yourself.
      url: https://github.com/jesperorb/node-api-proxy              
entities:
- class:
  - line
  rel:
  - self
  properties:
    name: Proxy
  links:
  - rel:
    - self
    href: deployment/proxy/
  - rel:
    - parent
    href: deployment/
links:
- rel:
  - self
  href: deployment/proxy/
- rel:
  - parent
  href: deployment/
...
