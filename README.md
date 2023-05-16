
# Setup 

1. Install `k3d` CLI (https://k3d.io/#installation)
2. `export KUBECONFIG=$PWD/kubeconfig.yaml`


# Cluster creation
Create using k3d command
```
k3d cluster create my-cluster
```

Or use a config file
```
k3d cluster create --config k3d.yaml
```

List all available clusters
```
kubectl config get contexts
```


# Check Kubernetes pods/nodes
```
kubectl get pods -A
kubectl get nodes
docker container ls
```


# Deleting clusters 
```
k3d cluster delete my-cluster
```



