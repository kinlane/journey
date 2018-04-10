---
class:
  - line
rel:
  - /rels/line
properties:
  name: Management
  sort: 9
  level: 1
  description: >-
    Information about how services are composed, limited, measured, reported
    upon, and managed consistently across all services, providing a consistent
    definition to how services get managed.
  tools:
    - name: Kong
      description: Kong was created to secure, manage and extend Microservices & APIs. Kong is powered by the battle-tested tech of NGINX and Cassandra with a focus on scalability, high performance & reliability. Kong runs in production at Mashape handling billions of requests to over ten thousand APIs.
      url: https://getkong.org/
    - name: Tyk
      description: An open source, lightweight, fast and scalable API Gateway. Set rate limiting, request throttling, and auto-renewing request quotas to manage how your users access your API. Tyk supports access tokens, HMAC request signing, basic authentication and OAuth 2.0 to integrate old and new services easily. Tyk can record and store detailed analytics which can be segmented by user, error, endpoint and client ID across multiple APIs and versions. Integrate your existing or new applications with Tyk using a simple REST API, Tyk even support hot-reloads so you can introduce new services without downtime.
      url: http://tyk.io/     
  services:
    - name: Axway
      description: Axway, acquired API Gateway vendor, Vordel, to complement its existing MFT and B2B Gateway products. Axways suite of products enables enterprise to govern the flow of data within and across the edge of the enterprise, unlocking the tremendous value this can bring to business interactions. Axway API Management offers the enterprise-grade API management architecture with the security to protect sensitive data, control access and support integration to a wide range of on-premise and cloud-based applications.
      url: https://www.axway.com/
    - name: Amazon API Gateway
      description: Amazon API Gateway is a fully managed service that makes it easy for developers to create, publish, maintain, monitor, and secure APIs at any scale. With a few clicks in the AWS Management Console, you can create an API that acts as a “front door” for applications to access data, business logic, or functionality from your back-end services, such as workloads running on Amazon Elastic Compute Cloud (Amazon EC2), code running on AWS Lambda, or any web application.
      url: https://aws.amazon.com/api-gateway/            
entities:
  - class:
      - line
    rel:
      - '/rels/line '
    properties:
      - name: Management
    links:
      - rel:
          - self
        href: /journey/management/
links:
  - rel:
      - self
    href: /management/
---
