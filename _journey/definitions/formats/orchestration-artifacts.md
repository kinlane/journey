---
class:
- stop
rel:
- self
properties:
  name: Orchestration Artifacts
  sort: 154
  level: 3
  description: Being organized regarding how Jenkins, and other CI/CD configuration files are stored, configured, audited, and used across the lifecycle. Organized centrally, audited, and tracked upon across deployments and builds looking for patterns and eliminating unhealthy practices.
  tools:
    - name: Jenkinsfile
      description: A Jenkinsfile is a text file that contains the definition of a Jenkins Pipeline and is checked into source control. Consider the following Pipeline which implements a basic three-stage continuous delivery pipeline.
      url: https://jenkins.io/doc/book/pipeline/jenkinsfile/
    - name: circle.yml
      description: CircleCI automatically infers settings from your code, so it’s possible you won’t need to add any custom configuration. If you do need to tweak settings, you can create a circle.yml in your project’s root directory and CircleCI will read it each time it runs a build. Use the following sections to set up your circle.yml file.
      url: https://circleci.com/docs/1.0/configuration/      
entities:
- class:
  - stop
  rel:
  - self
  properties:
    name: Orchestration Artifacts
  links:
  - rel:
    - self
    href: definitions/formats/orchestration-artifacts.md
  - rel:
    - parent
    href: definitions/formats/
links:
- rel:
  - self
  href: definitions/formats/orchestration-artifacts.md
- rel:
  - parent
  href: definitions/formats/
...
