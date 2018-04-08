---
class:
- stop
rel:
- self
properties:
  name: Session Management
  sort: 2278
  level: 3
  description: API should pass session-based authentication, either by session token
    via a POST or by API key as a POST body argument or as a cookie, avoiding usernames,
    passwords, session tokens, and API keys in the URL
entities:
- class:
  - stop
  rel:
  - self
  properties:
    name: Session Management
  links:
  - rel:
    - self
    href: security/authentication-considerations/session-management.md
  - rel:
    - parent
    href: security/authentication-considerations/
links:
- rel:
  - self
  href: security/authentication-considerations/session-management.md
- rel:
  - parent
  href: security/authentication-considerations/
...
