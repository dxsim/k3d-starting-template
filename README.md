# K3D cluster setup 


## Setup 
---
1. Install `k3d` CLI (https://k3d.io/#installation)
2. `export KUBECONFIG=$PWD/kubeconfig.yaml`


## Cluster creation
---
Three seperate ways to deploy your k3d cluster
* Create using the basic k3d command
    - `k3d cluster create my-cluster`

* Or use a config file
    - `k3d cluster create --config k3d.yaml`

* Or use terraform deployment
    - `terraform init`
    - `terraform apply`

* Destroy terraform deployment
    - `terraform destroy`
    
## List all available clusters
---
```
kubectl config get-contexts
```


## Check Kubernetes pods/nodes
---
```
kubectl get pods -A
kubectl get nodes
docker container ls
```


## Deleting clusters
---
```
k3d cluster delete my-cluster
```



