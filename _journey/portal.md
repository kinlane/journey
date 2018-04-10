---
class:
  - line
rel:
  - /rels/line
properties:
  name: Portal
  sort: 10
  level: 1
  description: >-
    The strategy for how all services are required to be published to one or many public, private, and partner developer portals. Providing a single location where all services can be accessed, with accompanying documentation and other essential building blocks of API operations.
  services:
    - name: Github Pages
      description: Websites for you and your projects. Hosted directly from your GitHub repository. Just edit, push, and your changes are live.
      url: https://pages.github.com/
    - name: APIMATIC Developer Experience Portal
      description: Instantly build an API Portal with SDKs, Live Code Samples, Test Cases, API Transformation and language specific Docs & Reference - tailored for your API.
      url: https://apimatic.io/developer-experience-portal     
  tools:
    - name: Jekyll
      description: Jekyll is a simple, blog-aware, static site generator for personal, project, or organization sites.
      url: https://jekyllrb.com/
    - name: Minimum Viable API Documentation Template
      description: An open source API portal template that can be forked and turned into the portal for any API platform.
      url: https://launchany.github.io/mvd-template/    
entities:
  - class:
      - line
    rel:
      - '/rels/line '
    properties:
      - name: Portal
    links:
      - rel:
          - self
        href: /journey/portal/
links:
  - rel:
      - self
    href: /portal/
---
