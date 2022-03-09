# AZURE DevOps challenge

Problem Statement:  Create a sample application using any technology along with microservices to demonstrate implementation of the DevOps principle using Azure services. Establish a pipeline for continuous integration, continuous testing, and continuous deployment.

Flow:

- ASP.NET Web application creation
	- DockerFile creation
- Push changes in Azure Repos (Along with DockerFile)
- Build and Push Image (ACR Repository)
- Deploy (AKS)
	- Creation of deployment.yml and service.yml files

![image](https://user-images.githubusercontent.com/79752341/157399500-c0d177df-36ef-4907-b61b-36e3950aec12.png)


Commands:

// This will allow to track new POD creation

kubectl get pods --watch

// We will then install the kubectl tool

az aks install-cli --install-location=./kubectl

// This allows kubectl to connect to the Kubernetes cluster

az aks get-credentials --resource-group devopsmela-rg --name devopsmelaAKS 

Pre-defined Variables:

$(Pipeline.Workspace)
	- The local path on the agent where all folders for a given build pipeline are created.


Web App:

![image](https://user-images.githubusercontent.com/79752341/157399678-22df8583-c0b7-42e0-80a5-2a368f13f335.png)

# Full docmentation in PDF inside. 
