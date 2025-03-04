# Azure Resource Manager and ARM Templates

![#f03c15](https://placehold.co/15x15/f03c15/f03c15.png) **Important**
---
- **Azure Resource Manager (ARM)** is the core service that handles the deployment and management of Azure resources. It enables you to create, update, and delete resources in your Azure environment.
- ARM is involved every time you interact with your Azure resources, whether through tools, APIs, or SDKs.
- ARM authenticates and authorizes user requests, ensuring consistent results across all Azure management tools.

![#c5f015](https://placehold.co/15x15/c5f015/c5f015.png) **Supporting Details**
---
- **Declarative Templates**: ARM allows you to manage infrastructure using **declarative templates** instead of scripting. A **Resource Manager template** (a JSON file) defines what resources you want to deploy in Azure.
- **Group Management**: Manage and monitor all resources for a solution as a group rather than individually.
- **Re-deployability**: You can redeploy resources across the development lifecycle with confidence that the resources will be deployed in a consistent state.
- **Resource Dependencies**: ARM ensures resources are deployed in the correct order, considering their dependencies.
- **RBAC Integration**: Role-Based Access Control (RBAC) is integrated into ARM for managing access control across services.
- **Resource Organization**: You can apply **tags** to resources to logically organize them and track costs based on those tags.

![#1589F0](https://placehold.co/15x15/1589F0/1589F0.png) **Examples/ Facts**
---
- **Infrastructure as Code**: With Azure Cloud Shell, PowerShell, or Azure CLI, you can manage infrastructure as code. ARM templates and **Bicep** are two examples of using infrastructure as code.
- **ARM Templates**:
    - Use **JSON** to describe the resources you want in a declarative format.
    - **Repeatable Deployments**: Deploy consistent environments by using the same ARM template multiple times.
    - **Orchestration**: ARM orchestrates the creation of dependent resources in the correct order and can deploy resources in parallel for faster results.
    - **Modularity**: Break templates into smaller, reusable components. You can nest templates within each other to deploy complex environments.
    - **Extensibility**: Add **PowerShell** or **Bash** scripts within ARM templates for further customization during deployment.

- **Bicep**:
    - **Simpler Syntax**: Bicep provides a more concise and readable alternative to ARM templates written in JSON.
    - **Support for All Resource Types**: Bicep supports all Azure services, including both preview and GA versions.
    - **Repeatable Results**: Bicep files are **idempotent**, ensuring consistent deployments.
    - **Orchestration**: Like ARM, Bicep leverages ARM to handle resource dependencies and deploy in parallel.
    - **Modular**: Bicep code can be broken down into manageable **modules** for reusable deployment configurations.

