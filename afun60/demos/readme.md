# Technical Demonstrations

* Use https://shell.azure.com 
* Ensure that your kubectl is connected to your AKS cluster : az aks get-credentials -n <aks-name> -g <resource-group>

| [README](/afun60/README.md) | [Slides](/afun60/slides/README.md) | [Demos](/afun60/demos/README.md) | [AKS Deployment](/afun60/aks/README.md) | 
|--------|-------|------------|-----------|

## Demo 1 - ACI (time permittting)

* az container create -n mycontainer --image microsoft/aci-helloworld -g myResourceGroup --ip-address public

## Demo 2 - App Service

* Portal : Create New Web App for Containers on Linux
* Location: EASTUS
* FREE Service Plan
* SET microsoft/aci-helloworld as the image

## Demo 3 - AKS

Get the deployment.yaml from a running pod

* kubectl get pods
* kubectl get pod <insert-2nd-to-last-pod-name-here> -o yaml 

Talk through the yaml deployment file, addressing the Enviroment variables set and the container image used.

