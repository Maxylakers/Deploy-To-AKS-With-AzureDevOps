# Deploy-to-AKS

Repository for showcasing the deployment from Azure DevOps Pipelines to Azure Kubernetes Service Using Azure Container Registry from scratch.

Few outputs can be found in the screenshots folder here in the project and here: https://dev.azure.com/nnangmathew/Dotnet-AKS-Deployment/_build

 
 We make a deployment for this image we build to Azure Container Reistry to run on Azure Kubernetes Service using the Azure DevOps pipeline.

 The use of Azure DevOps Environments has been used to serve as an authentication mechanism in place of Service Connections and a single pane of view for state of the deployments on the Azure portal.

 A marketplace extension called Replace Tokens was also used to "replace tokens" as a task in the Azure pipelines. This helps to automate the the number of replicas in the Kubernetes deployment.yml file once specified in the azure-pipelines.yml file. This can be found in the market place: https://marketplace.visualstudio.com/azuredevops

 Finally, detached the intially created managed identity for AKS to access ACR with imagePullSecrets as found here: https://learn.microsoft.com/en-us/azure/aks/cluster-container-registry-integration?toc=%2Fazure%2Fcontainer-registry%2Ftoc.json&bc=%2Fazure%2Fcontainer-registry%2Fbreadcrumb%2Ftoc.json&tabs=azure-cli 