---
class:
- stop
rel:
- self
properties:
  name: Sec-WebSocket-Version (RFC 6455)
  sort: 621
  level: 2
  description: 'The Sec-WebSocket-Version header field is used in the WebSocket opening
    handshake. It is sent from the client to the server to indicate the protocol version
    of the connection. This enables servers to correctly interpret the opening handshake
    and subsequent data being sent from the data, and close the connection if the
    server cannot interpret that data in a safe manner. The Sec-WebSocket-Version
    header field is also sent from the server to the client on WebSocket handshake
    error, when the version received from the client does not match a version understood
    by the server. In such a case, the header field includes the protocol version(s)
    supported by the server. '
entities:
- class:
  - stop
  rel:
  - self
  properties:
    name: Sec-WebSocket-Version (RFC 6455)
  links:
  - rel:
    - self
    href: design/headers/sec-websocket-version-rfc-6455.md
  - rel:
    - parent
    href: design/headers/
links:
- rel:
  - self
  href: design/headers/sec-websocket-version-rfc-6455.md
- rel:
  - parent
  href: design/headers/
...
