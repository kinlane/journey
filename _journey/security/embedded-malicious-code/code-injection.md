---
class:
- stop
rel:
- self
properties:
  name: Code Injection
  sort: 1
  level: 2
  description: Attack types which consist of injecting code that is then interpreted/executed
    by the application, exploiting poor handling of untrusted data, and usually made
    possible due to a lack of proper input/output data validation.
entities:
- class:
  - stop
  rel:
  - self
  properties:
    name: Code Injection
  links:
  - rel:
    - self
    href: security/embedded-malicious-code/code-injection.md
  - rel:
    - parent
    href: security/embedded-malicious-code/
links:
- rel:
  - self
  href: security/embedded-malicious-code/code-injection.md
- rel:
  - parent
  href: security/embedded-malicious-code/
...
