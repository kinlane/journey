---
class:
- stop
rel:
- self
properties:
  name: Format String Attack
  sort: 9
  level: 2
  description: Occurring when the submitted data of an input string is evaluated as
    a command, allowing the execution of code, to read the stack, or cause a segmentation
    fault, causing behaviors that could compromise the system.
entities:
- class:
  - stop
  rel:
  - self
  properties:
    name: Format String Attack
  links:
  - rel:
    - self
    href: security/embedded-malicious-code/format-string-attack.md
  - rel:
    - parent
    href: security/embedded-malicious-code/
links:
- rel:
  - self
  href: security/embedded-malicious-code/format-string-attack.md
- rel:
  - parent
  href: security/embedded-malicious-code/
...
