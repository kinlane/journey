---
class:
- stop
rel:
- self
properties:
  name: HTTP Long Polling
  sort: 22
  level: 2
  description: HTTP long polling, where the client polls the server requesting new
    information. The server holds the request open until new data is available. Once
    available, the server responds and sends the new information. When the client
    receives the new information, it immediately sends another request, and the operation
    is repeated. This effectively emulates a server push feature.
entities:
- class:
  - stop
  rel:
  - self
  properties:
    name: HTTP Long Polling
  links:
  - rel:
    - self
    href: real-time/protocols/http-long-polling.md
  - rel:
    - parent
    href: real-time/protocols/
links:
- rel:
  - self
  href: real-time/protocols/http-long-polling.md
- rel:
  - parent
  href: real-time/protocols/
...
