---
class:
- stop
rel:
- self
properties:
  name: MERGE (RFC 3253)
  sort: 282
  level: 2
  description: 'The MERGE method performs the logical merge of a specified version
    (the "merge source") into a specified version-controlled resource (the "merge
    target"). If the merge source is neither an ancestor nor a descendant of the DAV:checked-in
    or DAV:checked-out version of the merge target, the MERGE checks out the merge
    target (if it is not already checked out) and adds the URL of the merge source
    to the DAV:merge-set of the merge target. '
entities:
- class:
  - stop
  rel:
  - self
  properties:
    name: MERGE (RFC 3253)
  links:
  - rel:
    - self
    href: design/http-request-methods/merge-rfc-3253.md
  - rel:
    - parent
    href: design/http-request-methods/
links:
- rel:
  - self
  href: design/http-request-methods/merge-rfc-3253.md
- rel:
  - parent
  href: design/http-request-methods/
...
