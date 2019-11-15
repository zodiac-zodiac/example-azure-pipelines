# [:] Using SourceClear via Azure Pipelines running Linux Bash

1. Create a `azure-pipelines.yml` like [so](azure-pipelines.yml) for Azure Pipelines.
1. On AzureDevOps. At your project. Go to `Pipelines` > `Builds` > `+ New` > `New build pipeline` to connect your repository to Azure Pipelines. You may be immediately prompted to add a new build pipeline if you have no existing pipelines. 
1. We'll [do this](azure-pipelines.yml#L17-L18) as the equivalent of [CI script](https://help.veracode.com/reader/hHHR3gv0wYc2WbCclECf_A/_p_RJqZHXQ4S5pkjSXCrzQ) for Linux Bash.
1. On AzureDevOps. At your project. Go to `Pipelines` > `Builds` > `Edit` > `Variables` and add a new secret with the name of `SRCCLR_API_TOKEN`. We'll use the name of the environment variable SourceClear expects for consistency.
1. [Declare the `SRCCLR_API_TOKEN` secret](azure-pipelines.yml#L12-L14). 
1. Run the Azure Pipeline and enjoy!
