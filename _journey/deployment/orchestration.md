---
class:
- line
rel:
- self
properties:
  name: Orchestration
  sort: 1487
  level: 2
  description: Defining what the build, syndication, and orchestration of service
    deployments and integrations look like, and are executed, realizing a more organized
    and effective continuous integration and deployment workflow.
  service:
    - name: Jenkins
      description: An award-winning, cross-platform, continuous integration and continuous delivery application.
      url: https://jenkins.io/  
    - name: CircleCI
      description: Automated build, test &amp; deployment for public &amp; private projects.
      url: https://circleci.com/        
entities:
- class:
  - line
  rel:
  - self
  properties:
    name: Orchestration
  links:
  - rel:
    - self
    href: deployment/orchestration/
  - rel:
    - parent
    href: deployment/
links:
- rel:
  - self
  href: deployment/orchestration/
- rel:
  - parent
  href: deployment/
...
