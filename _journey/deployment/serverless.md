---
class:
- line
rel:
- self
properties:
  name: Serverless
  sort: 1441
  level: 2
  description: Powering the serverless deployment of services, using scalability scripts
    and functions to drive each service, and individual API paths.
  tools:
    - name: Apache OpenWhisk
      description: Apache OpenWhisk (Incubating) is a serverless, open source cloud platform that executes functions in response to events at any scale.
      url: https://openwhisk.apache.org/
  services:
    - name: AWS Lambda
      description: AWS Lambda is a zero-administration compute platform for back-end web developers that runs your code for you in the AWS cloud and provides you with a fine-grained pricing structure. AWS Lambda runs your back-end code on its own AWS compute fleet of Amazon Elastic Compute Cloud (Amazon EC2) instances across multiple Availability Zones in a region, which provides the high availability, security, performance, and scalability of the AWS infrastructure.
      url: http://docs.aws.amazon.com/lambda/   
entities:
- class:
  - line
  rel:
  - self
  properties:
    name: Serverless
  links:
  - rel:
    - self
    href: deployment/serverless/
  - rel:
    - parent
    href: deployment/
links:
- rel:
  - self
  href: deployment/serverless/
- rel:
  - parent
  href: deployment/
...
