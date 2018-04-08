---
class:
- stop
rel:
- self
properties:
  name: Websub
  sort: 3397
  level: 3
  description: Websub is an open protocol for distributed publish/subscribe communication
    on the Internet. Initially designed to extend the Atom (and RSS) protocols for
    data feeds, the protocol can be applied to any data type (e.g. HTML, text, pictures,
    audio, video) as long as it is accessible via HTTP. Its main purpose is to provide
    real-time notifications of changes, which improves upon the typical situation
    where a client periodically polls the feed server at some arbitrary interval.
    In this way, PubSubHubbub provides pushed HTTP notifications without requiring
    clients to spend resources on polling for changes.
entities:
- class:
  - stop
  rel:
  - self
  properties:
    name: Websub
  links:
  - rel:
    - self
    href: real-time/protocols/websub.md
  - rel:
    - parent
    href: real-time/protocols/
links:
- rel:
  - self
  href: real-time/protocols/websub.md
- rel:
  - parent
  href: real-time/protocols/
...
