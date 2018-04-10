---
class:
- stop
rel:
- self
properties:
  name: IDE Plugin
  sort: 182
  level: 3
  description: Providing integration with existing integrated development environments
    (IDE), giving developers API discovery, documentation, and integration tooling
    within the IDE.
  services:
    - name: Azure Visual Studio
      description: Continuous integration and deployment tools automatically build and test your code, then deploy your changes directly to Azure.
      url: https://www.visualstudio.com/vs/features/azure/
    - name: Google Plugin for Eclipse
      description: A plugin for the Google Cloud environment for working within the Eclipse IDE.
      url: https://cloud.google.com/eclipse/docs/migrating-gpe     
    - name: AWS Toolkit for Eclipse
      description: The AWS Toolkit for Eclipse is an open source plug-in for the Eclipse Java IDE that makes it easier for developers to develop, debug, and deploy Java applications using Amazon Web Services.
      url: https://aws.amazon.com/eclipse/      
entities:
- class:
  - stop
  rel:
  - self
  properties:
    name: IDE Plugin
  links:
  - rel:
    - self
    href: definitions/environment/ide-plugin.md
  - rel:
    - parent
    href: definitions/environment/
links:
- rel:
  - self
  href: definitions/environment/ide-plugin.md
- rel:
  - parent
  href: definitions/environment/
...
