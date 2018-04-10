---
class:
- line
rel:
- self
properties:
  name: Compute
  sort: 1328
  level: 2
  description: How is the underlying compute delivered for each service using containers,
    serverless, cloud, and on-premise infrastructure.
  services:
    - name: Amazon EC2
      description: Amazon Elastic Compute Cloud (Amazon EC2) is a web service that provides secure, resizable compute capacity in the cloud. It is designed to make web-scale cloud computing easier for developers.
      url: https://aws.amazon.com/ec2/
    - name: Azure Compute
      description: Access cloud compute capacity, virtualization, and scale on demand—and only pay for the resources you use.
      url: https://azure.microsoft.com/en-us/product-categories/compute/
    - name: Google Compute Engine
      description: Google Compute Engine delivers virtual machines running in Google's innovative data centers and worldwide fiber network. Compute Engine's tooling and workflow support enable scaling from single instances to global, load-balanced cloud computing.
      url: https://cloud.google.com/compute/            
entities:
- class:
  - line
  rel:
  - self
  properties:
    name: Compute
  links:
  - rel:
    - self
    href: deployment/compute/
  - rel:
    - parent
    href: deployment/
links:
- rel:
  - self
  href: deployment/compute/
- rel:
  - parent
  href: deployment/
...
