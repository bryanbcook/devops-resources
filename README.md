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

- [YAML Schema Reference](https://learn.microsoft.com/en-us/azure/devops/pipelines/yaml-schema/?view=azure-pipelines&viewFallbackFrom=azure-devops&tabs=schema%2Cparameter-schema)
- [Predefined Pipeline Variables](https://learn.microsoft.com/en-us/azure/devops/pipelines/build/variables?view=azure-devops&tabs=yaml)
- [Logging commands](https://learn.microsoft.com/en-us/azure/devops/pipelines/scripts/logging-commands?view=azure-devops&tabs=bash)
- [Expressions](https://learn.microsoft.com/en-us/azure/devops/pipelines/process/expressions?view=azure-devops)
- [Templates](https://learn.microsoft.com/en-us/azure/devops/pipelines/process/templates?view=azure-devops&pivots=templates-includes)
- [Runtime parameters](https://learn.microsoft.com/en-us/azure/devops/pipelines/process/runtime-parameters?view=azure-devops&tabs=script)
- [Pipeline run sequence](https://learn.microsoft.com/en-us/azure/devops/pipelines/process/runs?view=azure-devops)
- [Tasks Reference](https://learn.microsoft.com/en-us/azure/devops/pipelines/tasks/reference/?view=azure-pipelines)
- [Tasks (source-code)](https://github.com/microsoft/azure-pipelines-tasks/tree/master/Tasks)
  - [AzureKeyVaultV2](https://github.com/microsoft/azure-pipelines-tasks/tree/master/Tasks/AzureKeyVaultV2) - contains a "prejob"

### Build Agents

- [actions/runner-images](https://github.com/actions/runner-images)
- [microsoft/azure-pipelines-agent](https://github.com/microsoft/azure-pipelines-agent)
  - [Handlers](https://github.com/microsoft/azure-pipelines-agent/tree/master/src/Agent.Worker/Handlers)

### Azure DevOps APIs

- [Azure DevOps REST API (Home)](https://learn.microsoft.com/en-us/rest/api/azure/devops/?view=azure-devops-rest-7.2)
- [azure-devops-extension-api package](https://learn.microsoft.com/en-us/javascript/api/azure-devops-extension-api/)
- [.NET SDK](https://learn.microsoft.com/en-us/dotnet/api/?view=azure-devops-dotnet&preserve-view=true)

PAT Tokens:

- [List of available scopes](https://learn.microsoft.com/en-us/azure/devops/integrate/get-started/authentication/oauth?view=azure-devops#scopes)
 
### Extensions Development

- [Extensions manifest reference](https://learn.microsoft.com/en-us/azure/devops/extend/develop/manifest?toc=%2Fazure%2Fdevops%2Fmarketplace-extensibility%2Ftoc.json&view=azure-devops)
- [tasks.schema.json](https://github.com/Microsoft/azure-pipelines-task-lib/blob/master/tasks.schema.json)
- [microsoft/azure-pipelines-task-lib](https://github.com/microsoft/azure-pipelines-task-lib/tree/master)
  - [node](https://github.com/microsoft/azure-pipelines-task-lib/tree/master/node)
  - [powershell](https://github.com/microsoft/azure-pipelines-task-lib/tree/master/powershell)
