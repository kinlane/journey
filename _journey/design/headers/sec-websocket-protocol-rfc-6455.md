---
class:
- stop
rel:
- self
properties:
  name: Sec-WebSocket-Protocol (RFC 6455)
  sort: 619
  level: 2
  description: 'The Sec-WebSocket-Protocol header field is used in the WebSocket opening
    handshake. It is sent from the client to the server and back from the server to
    the client to confirm the subprotocol of the connection. This enables scripts
    to both select a subprotocol and be sure that the server agreed to serve that
    subprotocol. '
entities:
- class:
  - stop
  rel:
  - self
  properties:
    name: Sec-WebSocket-Protocol (RFC 6455)
  links:
  - rel:
    - self
    href: design/headers/sec-websocket-protocol-rfc-6455.md
  - rel:
    - parent
    href: design/headers/
links:
- rel:
  - self
  href: design/headers/sec-websocket-protocol-rfc-6455.md
- rel:
  - parent
  href: design/headers/
...
