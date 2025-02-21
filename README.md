# Kubernetes on Azure

This is the repo that contains multiple workshops for Kubernetes on Azure and the supporting code examples.

## Prerequisites

### Prior knowledge 
To be successful at getting the most out of these workshops you will need the following prior knowledge

* A basic understanding of Linux
* Be able to read bash scripts
* Have a basic knowledge of what a container is 

### Equipment
To be able to run the labs in the workshops you will need the following 

* A bash shell (WSL works fine if you are a windows user)
  I have written a [post](https://medium.com/devopslinks/windows-for-a-linux-guy-823276351826) on how to get WSL configured for the workshops.  
  If a bash shell is not available to you please use [azure cloud shell](https://azure.microsoft.com/en-au/features/cloud-shell/?WT.mc_id=aksworkshop-github-sccoulto)

* An Azure account that has access to create service principals

If you dont have an Azure account and want to run the workshops, you can sign up for an [Azure trial](https://azure.microsoft.com/en-us/offers/ms-azr-0044p/?WT.mc_id=aksworkshop-github-sccoulto) that will give you free credit to complete the workshop.

### Installed software
There are a few packages we will need to run the labs so we will need to install the following

* [Azure cli](https://docs.microsoft.com/cli/azure/install-azure-cli?view=azure-cli-latest&?WT.mc_id=aksworkshop-github-sccoulto)
* [kubectx](https://github.com/ahmetb/kubectx)
* jq (install from you package manager) 

## How to use the workshops
Each folder is named after a corresponding module in the workshop. Inside that folder is all the code examples for that module.

## Workshops 

At present there are four workshops in this repo. Each of them are designed for different lengths of time depending how long your time slot is to give the workshop.

### Kubernetes on Azure full workshop
This is the full workshop that covers Kubernetes 101, Helm, virtual kubelet and some basic istio topic. Below are the full list of topics

 Kubernetes 101
 
* Introduction into Kubernetes
* Kubernetes components 
* [Deploying Kubernetes on Azure](deploying-kubernetes-on-azure/code.md)
* [Pods, services and deployments](pods-services-deployments/code.md)
* [Rabc, roles and service accounts](rbac-roles-service-accounts/code.md) 
* [Stateful sets](statefull-sets/code.md)
* Kubernetes networking and service discovery
* [Load balancing and ingress control](ingress-controller/code.md)

 Helm

* Introduction into Helm
* Understanding charts
* [Deploying Helm on Kubernetes](installing-helm-on-kubernetes/code.md)
* Helm cli
* [Deploying a public chart](deploying-a-public-chart/code.md)
* [Writing our own chart](writing-our-own-chart/code.md)
* Helm and CNAB

 Kubernetes advanced topics

* [Virtual kubelet](virtual-node-with-virtual-kubelet/code.md)
* [Pod security context](pod-security-policy/code.md) 
* Introduction to istio
* Advanced application routing with istio(advanced-application-routing-with-istio/code.md)
* [Setting mTLS between application services with istio](mTLS-with-istio/code.md) 

This workshop takes about 6hrs to give as instructor lead workshop.  
The slides can be found [here](slides/full-workshop/Kubernetes-on-Azure.pdf)  


### Kubernetes 101
This workshop is the entry level into Azure Kubernetes service. In the workshop we will cover the topics listed above in the kubernetes 101 section. This will take approx 2hrs for an instructor to give.  

### Kubernetes and Helm 
This workshop covers the kubernetes 101 workshop and adds all the Helm modules listed above. 
The slides can be found [here](slides/kubernetes-helm/Kubernetes-helm.pdf).  
This workshop will take about 4hrs to complete  

### Advanced Kubernetes
This workshop adds the Kubernetes 101 modules with the advanced Kubernetes topics.  
The slides can be found [here](slides/kubernetes-advanced/Kubernetes-advanced.pdf)  
This workshop will take about 4hrs   

## Further reading
I have done a few blog posts on topics covered by this workshop for further . This list will continue to be updated.
* [Choosing the right container base image](https://dev.to/scottyc/i-cho-cho-chose-you-container-image-part-1-227p)
* [Pod security 101](https://medium.com/devopslinks/kubernetes-pod-security-101-15fe8cda829e)
* [Understading application routing with istio](https://itnext.io/understanding-application-routing-in-istio-aade30d594f4)

If there is something that is not covered in the workshops and you would like it to be. Please raise an issue on this repo and I will do my best to add it in where possible

