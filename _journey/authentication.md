---
class:
  - line
rel:
  - /rels/line
properties:
  name: Authentication
  sort: 8
  level: 1
  description: >-
    What is involved with authentication across all services, including
    key-based approaches, basic authentication, JWT, and OAuth solutions.
  x: 0
  y: 6
  color: 68077E
  direction: S  
  tools:     
  services:
    - name: Auth0
      description: Authenticate and authorize apps and APIs with any popular identity provider (enterprise, social or custom) running on any popular software stack on any popular device or cloud with Auth0's identity-as-a-service. Run from the Auth0 public cloud service, from a private cloud instance, or on-prem. Auth0 allows developers to replace painfully brittle in-app auth code with a call to an easy-to-use cloud service. Auth0 is particularly useful in eliminating the pain of dealing with a complex identity environment. Auth0 further allows IT to quickly set up SSO for any SAML-compliant 3rd party app (SaaS or on-prem).
      url: https://auth0.com/
    - name: Okta
      description: Okta is the foundation for secure connections between people and technology. By harnessing the power of the cloud, Okta allows people to access applications on any device at any time, while still enforcing strong security protections. It integrates directly with an organization's existing directories and identity systems, as well as 4,000+ applications.
      url: https://www.okta.com/ 
entities:
  - class:
      - line
    rel:
      - '/rels/line '
    properties:
      - name: Authentication
    links:
      - rel:
          - self
        href: /journey/authentication/
links:
  - rel:
      - self
    href: /authentication/
---
