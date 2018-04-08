---
class:
- stop
rel:
- self
properties:
  name: ACL (RFC 3744)
  sort: 256
  level: 2
  description: 'The ACL method modifies the access control list (which can be read
    via the DAV:acl property) of a resource. Specifically, the ACL method only permits
    modification to ACEs that are not inherited, and are not protected. '
entities:
- class:
  - stop
  rel:
  - self
  properties:
    name: ACL (RFC 3744)
  links:
  - rel:
    - self
    href: design/http-request-methods/acl-rfc-3744.md
  - rel:
    - parent
    href: design/http-request-methods/
links:
- rel:
  - self
  href: design/http-request-methods/acl-rfc-3744.md
- rel:
  - parent
  href: design/http-request-methods/
...
