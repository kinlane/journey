---
class:
- stop
rel:
- self
properties:
  name: Repository
  sort: 186
  level: 3
  description: Management of all definitions within a version control system, using the underlying repository as a location to aggregate, store, and include API definitions into build pipelines.
  services:
    - name: Github
      description: GitHub is a web-based hosting service for version control using git. It is mostly used for computer code. It offers all of the distributed version control and source code management functionality of Git as well as adding its own features.
      url: https://github.com/
    - name: Gitlab
      description: GitLab is a web-based Git-repository manager with wiki and issue-tracking features, using an open-source license, developed by GitLab Inc.
      url: https://gitlab.com/
    - name: Bitbucket
      description: Bitbucket is a web-based version control repository hosting service owned by Atlassian, for source code and development projects that use either Mercurial or Git revision control systems.
      url: https://bitbucket.org/
    - name: Team Foundation Server
      description: Store and collaborate on code with unlimited private repositories. Use Git for distributed version control or Team Foundation version control (TFVC) for centralized version control. Collaborate on code easily with pull requests and code reviews. Manage permissions and policies to secure your repositories.
      url: https://www.visualstudio.com/tfs/                   
entities:
- class:
  - stop
  rel:
  - self
  properties:
    name: Github
  links:
  - rel:
    - self
    href: definitions/environment/github.md
  - rel:
    - parent
    href: definitions/environment/
links:
- rel:
  - self
  href: definitions/environment/github.md
- rel:
  - parent
  href: definitions/environment/
...
