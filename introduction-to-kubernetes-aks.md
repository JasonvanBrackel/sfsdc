# Introduction To Kubernetes with Azure Kubernetes Service

## What is Kubernetes

## Why Should I Care
- Operators
- Developers
- They Won!?

## What is AKS
- Highly Available
- Fully Managed
- Backed by https://github.com/Azure/aks-engine

## Why AKS
- Your not a Kube Expert
- You don't want the hastle

## Why not AKS
- You want control
- You want newer features
- No Windows Yet
- No SLA
- https://azure.microsoft.com/en-in/support/legal/sla/kubernetes-service/v1_0/
- 43.8 hrs of downtime

## Deploying Azure Kubernetes Service

- ARM Templates
- Azure Portal
- Azure CLI
- Infrastructure as Code
  - Terraform
  - Pulumi
- Rancher

## Let's talk what is Kubernetes

- Concepts Underlying the Cloud Controller Manager

## Attaching to Kubernetes

- Get the cli
- az aks install-cli
- Enable source code completion in bash
- echo 'source <(kubectl completion bash)' >>~/.bashrc
- Get Kubeconfig from az cli
- az aks get-credentials --resource-group myResourceGroup --name myAKSCluster
- Whats in a Kubeconfig
- The KUBECONFIG variable
- Useful tools
  - Kubectx
  - Kube-ps1

## A Simple Example

- Deploy nginx
kubectl run nginx-web --image nginx
- Exec into the container
kubectl exec nginx-web-84dc48d749-md2gl -it /bin/sh
- curl the output
- Review the Namespace
- Review the ReplicaSet
- Review the Pod
- Review the Deployment
- Review Labels
- Review Selectors

## Adding a Service

- Add a service for nginx
- Create a Load Balancer Service
- Service Types
- Protocol Support

## Adding an Ingress Controller

- xip.io example


## Look at Nodes

- Nodes
- Labels
- Taints and Tolerations

## Azure Specific Features

- Node Pools
- Virtual Nodes
- VM Scale Sets
- Http Application Routing


## Learn More

- [AKS Engine](https://github.com/Azure/aks-engine)


