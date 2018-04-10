---
class:
  - line
rel:
  - /rels/line
properties:
  name: Client
  sort: 30
  level: 1
  description: >-
    Information about clients being used to interface with and work with the service, allowing it to be put to use without code, in the browser, on the desktop, or some other installable client that can be used by anyone.
  x: 0
  y: 20
  color: BA801A
  direction: S      
  services:
    - name: Postman
      description: Postman on Chrome is the most efficient way to test, develop and document APIs. Create complex requests, go back in time and view results in a beautiful way. Postman has more than 80 features to help you at every step. Our user base is growing rapidly and with more tools in the pipeline, Postman aims to provide the most comprehensive API development and testing solution to developers.
      url: http://www.getpostman.com/    
entities:
  - class:
      - line
    rel:
      - '/rels/line '
    properties:
      - name: Client
    links:
      - rel:
          - self
        href: /journey/client/
links:
  - rel:
      - self
    href: /client/
---
