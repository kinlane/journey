---
class:
- stop
rel:
- self
properties:
  name: Registry
  sort: 1369
  level: 3
  description: Establishing a container image registry with available container images,
    and instructions for how images are meant to be deployed in support of services.
  service:
    - name: Docker Hub
      description: Docker Hub. Dev-test pipeline automation, 100,000+ free apps, public and private registries.
      url: https://hub.docker.com/  
    - name: Google Container Registry
      description: Store your private Docker container images on GCP for fast, scalable retrieval and deployment. Container Registry is a private Docker repository that works with popular continuous delivery systems. It runs on GCP to provide consistent uptime on an infrastructure protected by Google's security. You pay only for storage and internet egress you use, there is no per-image fee.
      url: https://cloud.google.com/container-registry/
    - name: Azure Container Registry
      description: Azure Container Registry allows you to store images for all types of container deployments including DC/OS, Docker Swarm, Kubernetes, and Azure services such as App Service, Batch, Service Fabric, and others. Your DevOps team can manage the configuration of apps isolated from the configuration of the hosting environment.
      url: https://azure.microsoft.com/en-us/services/container-registry/
    - name: Amazon Elastic Container Registry
      description: Amazon Elastic Container Registry (ECR) is a fully-managed Docker container registry that makes it easy for developers to store, manage, and deploy Docker container images. Amazon ECR is integrated with Amazon Elastic Container Service (ECS), simplifying your development to production workflow. Amazon ECR eliminates the need to operate your own container repositories or worry about scaling the underlying infrastructure. Amazon ECR hosts your images in a highly available and scalable architecture, allowing you to reliably deploy containers for your applications. Integration with AWS Identity and Access Management (IAM) provides resource-level control of each repository. With Amazon ECR, there are no upfront fees or commitments. You pay only for the amount of data you store in your repositories and data transferred to the Internet.
      url: https://aws.amazon.com/ecr/                  
entities:
- class:
  - stop
  rel:
  - self
  properties:
    name: Image Registry
  links:
  - rel:
    - self
    href: deployment/containers/image-registry.md
  - rel:
    - parent
    href: deployment/containers/
links:
- rel:
  - self
  href: deployment/containers/image-registry.md
- rel:
  - parent
  href: deployment/containers/
...
