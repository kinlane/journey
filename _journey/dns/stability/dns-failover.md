---
class:
- stop
rel:
- self
properties:
  name: DNS Failover
  sort: 2
  level: 2
  description: Allowing for failover at the DNS level, providing redundancy and failover
    of
entities:
- class:
  - stop
  rel:
  - self
  properties:
    name: DNS Failover
  links:
  - rel:
    - self
    href: dns/stability/dns-failover.md
  - rel:
    - parent
    href: dns/stability/
links:
- rel:
  - self
  href: dns/stability/dns-failover.md
- rel:
  - parent
  href: dns/stability/
...