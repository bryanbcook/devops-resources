# DevOps Resources

My collection of useful DevOps resources

## Azure DevOps

### Training Sessions

  - [Microsoft Learn - Define and implement continuous integration](https://learn.microsoft.com/en-us/training/paths/az-400-define-implement-continuous-integration/)
  - [Microsoft Learn - Build applications with Azure DevOps](https://learn.microsoft.com/en-us/training/paths/build-applications-with-azure-devops/)
  - [Microsoft Learn - Deploy applications with Azure DevOps](https://learn.microsoft.com/en-us/training/paths/deploy-applications-with-azure-devops/)
  - [Microsoft Learn - Implement CI with Azure Pipelines and GitHub Actions](https://learn.microsoft.com/en-us/training/paths/az-400-implement-ci-azure-pipelines-github-actions/)
  - [Microsoft Learn - Implement a secure continuous deployment using Azure Pipelines](https://learn.microsoft.com/en-us/training/paths/az-400-implement-secure-continuous-deployment/)

### YAML Pipelines

My list of go-to pages during YAML development:

- [YAML Schema Reference](https://learn.microsoft.com/en-us/azure/devops/pipelines/yaml-schema/?view=azure-pipelines&viewFallbackFrom=azure-devops&tabs=schema%2Cparameter-schema): Describes the supported schema for pipelines, resources, jobs, etc.
- [Predefined Pipeline Variables](https://learn.microsoft.com/en-us/azure/devops/pipelines/build/variables?view=azure-devops&tabs=yaml): daily go-to resource for understanding the variables that are available in a pipeline execution and their possible values.
- [Logging commands](https://learn.microsoft.com/en-us/azure/devops/pipelines/scripts/logging-commands?view=azure-devops&tabs=bash): daily reference for `##vso` logging statements for creating variables, adding attachments, reporting failures.
- [Expressions](https://learn.microsoft.com/en-us/azure/devops/pipelines/process/expressions?view=azure-devops): data types and available functions available for custom conditions or compile-time expressions.
- [Templates](https://learn.microsoft.com/en-us/azure/devops/pipelines/process/templates?view=azure-devops&pivots=templates-includes): outlines how to use templates for stages, jobs, steps and variables.
- [Runtime parameters](https://learn.microsoft.com/en-us/azure/devops/pipelines/process/runtime-parameters?view=azure-devops&tabs=script): data-types supported for prompting users for values when queueing pipelines.
- [Pipeline run sequence](https://learn.microsoft.com/en-us/azure/devops/pipelines/process/runs?view=azure-devops): understanding the sequence of how the pipeline is executed is necessary to understand the differences between compile-time and run-time. Also provides insights on how agents and jobs execute.
- [Tasks Reference](https://learn.microsoft.com/en-us/azure/devops/pipelines/tasks/reference/?view=azure-pipelines): list of available built-in Azure DevOps tasks, provides different versions and supported syntax.
- [Tasks (source-code)](https://github.com/microsoft/azure-pipelines-tasks/tree/master/Tasks): deeper dive into the internal logic of the built-in tasks, useful for understanding how specific fields impact the execution. Also a good reference for building your own custom tasks.
  - [AzureKeyVaultV2](https://github.com/microsoft/azure-pipelines-tasks/tree/master/Tasks/AzureKeyVaultV2) - this task contains a "prejob" execution handler.

### Build Agents

- [actions/runner-images](https://github.com/actions/runner-images): contains installation scripts used to build a virtual machine to be used as a build-agent. 
- [microsoft/azure-pipelines-agent](https://github.com/microsoft/azure-pipelines-agent): source code for the build-agent software that executes a pipeline.
  - [Handlers](https://github.com/microsoft/azure-pipelines-agent/tree/master/src/Agent.Worker/Handlers): useful insight into how the build agent bootstraps the execution of a task (powershell, exe, nodejs, etc)

### Azure DevOps APIs

- [Azure DevOps REST API](https://learn.microsoft.com/en-us/rest/api/azure/devops/?view=azure-devops-rest-7.2): the SDKs and client libraries are wrappers around the REST API, outlines available endpoints, query parameters and schema for payloads and responses.
- [azure-devops-extension-api package](https://learn.microsoft.com/en-us/javascript/api/azure-devops-extension-api/): NodeJs wrapper library for the REST API.
- [.NET SDK](https://learn.microsoft.com/en-us/dotnet/api/?view=azure-devops-dotnet&preserve-view=true): .NET wrapper for the REST API.

PAT Tokens:

- [List of available scopes](https://learn.microsoft.com/en-us/azure/devops/integrate/get-started/authentication/oauth?view=azure-devops#scopes): useful for determining which permissions to grant to a PAT token. If you're buildnig a custom task, each method in the REST API indicates which scope it requires.
 
### Extensions Development

- [Extensions manifest reference](https://learn.microsoft.com/en-us/azure/devops/extend/develop/manifest?toc=%2Fazure%2Fdevops%2Fmarketplace-extensibility%2Ftoc.json&view=azure-devops): describes the schema for a custom extension.
- [tasks.schema.json](https://github.com/Microsoft/azure-pipelines-task-lib/blob/master/tasks.schema.json): describes the schema for a task within an extension.
- [microsoft/azure-pipelines-task-lib](https://github.com/microsoft/azure-pipelines-task-lib/tree/master): custom tasks rely on the capabilities of the task-lib to interact with task inputs, variables, output masking, etc
  - [node](https://github.com/microsoft/azure-pipelines-task-lib/tree/master/node)
  - [powershell](https://github.com/microsoft/azure-pipelines-task-lib/tree/master/powershell)

### Azure DevOps Product Team

- [Azure DevOps Roadmap][https://learn.microsoft.com/en-us/azure/devops/release-notes/features-timeline]: follow the release by week to see the latest features.
- [Current Sprint][https://whatsprintis.it]: the ADO team releases roughly every 3 weeks. This shows the current sprint + week which can be used as a soft indicator for the timing of the next feature release.

### Wiki

- [list of markdown emojis](https://gist.github.com/rxaviers/7360908)
