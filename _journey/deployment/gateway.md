---
class:
- line
rel:
- self
properties:
  name: Gateway
  sort: 1118
  level: 2
  description: A heavier duty implementation that provides a doorway to new or existing
    services, providing more robust solutions for accessing backend services via web
    APIs.
  services:
    - name: Amazon API Gateway
      description: Amazon API Gateway is a fully managed service that makes it easy for developers to create, publish, maintain, monitor, and secure APIs at any scale. With a few clicks in the AWS Management Console, you can create an API that acts as a “front door” for applications to access data, business logic, or functionality from your back-end services, such as workloads running on Amazon Elastic Compute Cloud (Amazon EC2), code running on AWS Lambda, or any web application.
      url: https://aws.amazon.com/api-gateway/   
entities:
- class:
  - line
  rel:
  - self
  properties:
    name: Gateway
  links:
  - rel:
    - self
    href: deployment/gateway/
  - rel:
    - parent
    href: deployment/
links:
- rel:
  - self
  href: deployment/gateway/
- rel:
  - parent
  href: deployment/
...
