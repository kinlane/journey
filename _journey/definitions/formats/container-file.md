---
class:
- stop
rel:
- self
properties:
  name: Container File
  sort: 152
  level: 3
  description: Leveraging and approaching management of the container configuration
    files used as part of the container deliver process.
  tools:
    - name: Dockerfile
      description: Docker can build images automatically by reading the instructions from a Dockerfile. A Dockerfile is a text document that contains all the commands a user could call on the command line to assemble an image. Using docker build users can create an automated build that executes several command-line instructions in succession.
      url: https://docs.docker.com/engine/reference/builder/
    - name: Kubernetes ConfigMap
      description: Many applications require configuration via some combination of config files, command line arguments, and environment variables. These configuration artifacts should be decoupled from image content in order to keep containerized applications portable. The ConfigMap API resource provides mechanisms to inject containers with configuration data while keeping containers agnostic of Kubernetes. ConfigMap can be used to store fine-grained information like individual properties or coarse-grained information like entire config files or JSON blobs.
      url: https://kubernetes-v1-4.github.io/docs/user-guide/configmap/     
entities:
- class:
  - stop
  rel:
  - self
  properties:
    name: Container File
  links:
  - rel:
    - self
    href: definitions/formats/container-file.md
  - rel:
    - parent
    href: definitions/formats/
links:
- rel:
  - self
  href: definitions/formats/container-file.md
- rel:
  - parent
  href: definitions/formats/
...
