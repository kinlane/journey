---
class:
- stop
rel:
- self
properties:
  name: Circuit Breakers
  sort: 7
  level: 2
  description: Allowing for a circuit breaker model to exist between a service, and
    it's backend dependencies, triggering when a backend service becomes unreliable
    or unavailable.
entities:
- class:
  - stop
  rel:
  - self
  properties:
    name: Circuit Breakers
  links:
  - rel:
    - self
    href: management/change/circuit-breakers.md
  - rel:
    - parent
    href: management/change/
links:
- rel:
  - self
  href: management/change/circuit-breakers.md
- rel:
  - parent
  href: management/change/
...
