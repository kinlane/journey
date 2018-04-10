---
class:
- line
rel:
- self
properties:
  name: Containers
  sort: 1366
  level: 2
  description: Providing standard practices for defining, deploying, and managing
    the deployment of services using common containerization services and tooling,
    making services as modular as scalable as they can be.
  tools:
    - name: Docker
      description: Docker is an open platform for developers and sysadmins to build, ship, and run distributed applications. Consisting of Docker Engine, a portable, lightweight runtime and packaging tool, and Docker Hub, a cloud service for sharing applications and automating workflows, Docker enables apps to be quickly assembled from components and eliminates the friction between development, QA, and production environments. As a result, IT can ship faster and run the same app, unchanged, on laptops, data center VMs, and any cloud.
      url: https://github.com/docker/docker-ce
    - name: Kubernetes
      description: Manage a cluster of Linux containers as a single system to accelerate Dev and simplify Ops. Kubernetes is an open source orchestration system for Docker containers. It handles scheduling onto nodes in a compute cluster and actively manages workloads to ensure that their state matches the users declared intentions. Using the concepts of labels and pods, it groups the containers which make up an application into logical units for easy management and discovery.
      url: https://github.com/kubernetes/kubernetes           
  service:
    - name: Docker
      description: Docker is an open platform for developers and sysadmins to build, ship, and run distributed applications. Consisting of Docker Engine, a portable, lightweight runtime and packaging tool, and Docker Hub, a cloud service for sharing applications and automating workflows, Docker enables apps to be quickly assembled from components and eliminates the friction between development, QA, and production environments. As a result, IT can ship faster and run the same app, unchanged, on laptops, data center VMs, and any cloud.
      url: https://www.docker.com/
    - name: Kubernetes
      description: Manage a cluster of Linux containers as a single system to accelerate Dev and simplify Ops. Kubernetes is an open source orchestration system for Docker containers. It handles scheduling onto nodes in a compute cluster and actively manages workloads to ensure that their state matches the users declared intentions. Using the concepts of labels and pods, it groups the containers which make up an application into logical units for easy management and discovery.
      url: http://kubernetes.io/          
entities:
- class:
  - line
  rel:
  - self
  properties:
    name: Containers
  links:
  - rel:
    - self
    href: deployment/containers/
  - rel:
    - parent
    href: deployment/
links:
- rel:
  - self
  href: deployment/containers/
- rel:
  - parent
  href: deployment/
...
