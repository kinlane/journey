---
class:
- stop
rel:
- self
properties:
  name: Digest (RFC 7616)
  sort: 4
  level: 2
  description: 'The Digest scheme is based on a simple challenge-response paradigm.
    The Digest scheme challenges using a nonce value and might indicate that username
    hashing is supported. A valid response contains an unkeyed digest of the username,
    the password, the given nonce value, the HTTP method, and the requested URI. '
entities:
- class:
  - stop
  rel:
  - self
  properties:
    name: Digest (RFC 7616)
  links:
  - rel:
    - self
    href: authentication/approaches/digest-rfc-7616.md
  - rel:
    - parent
    href: authentication/approaches/
links:
- rel:
  - self
  href: authentication/approaches/digest-rfc-7616.md
- rel:
  - parent
  href: authentication/approaches/
...
