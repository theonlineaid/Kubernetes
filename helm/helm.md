
# Instalation
```
sudo snap install helm --classic
helm version
# version.BuildInfo{Version:"v3.16.4", GitCommit:"7877b45b63f95635153b29a42c0c2f4273ec45ca", GitTreeState:"clean", GoVersion:"go1.22.7"}
```

## Create Helm FS
```
helm create my-first-chart
```

### Create Custom Template
```
kubectl create deploy my-deployment --image=nginx --dry-run=client -o yaml > templates/deployment.yaml
kubectl create service nodeport my-service --tcp=80:80 --dry-run=client -o yaml > templates/service.yaml
```

### Create Chart
```
helm install [first-relase] . // you can't take same name 
NAME: fchart-relase
LAST DEPLOYED: Sat Jan 11 17:11:26 2025
NAMESPACE: default
STATUS: deployed
REVISION: 1
TEST SUITE: None
```

### Check List of helm chart
```
helm list
```

### Check Helm Lint
```
helm lint .
```

### Check Helm manifast compiler
```
helm get manifest web-server
```
