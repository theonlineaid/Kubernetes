
## Instalation
```
sudo snap install helm --classic
helm version
version.BuildInfo{Version:"v3.16.4", GitCommit:"7877b45b63f95635153b29a42c0c2f4273ec45ca", GitTreeState:"clean", GoVersion:"go1.22.7"}
```

## Create Helm FS
```
helm create my-first-chart
```

# Create Custom Chart
```
kubectl create deploy my-deployment --image=nginx --dry-run=client -o yaml > templates/deployment.yaml

```