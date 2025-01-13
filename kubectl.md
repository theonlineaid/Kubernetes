
## CMD list of kubectl

``` bash
kubectl version
kubectl version --client

kubectl config view
kubectl cluster-info
kubectl get nodes

# those are same 
kubectl get pod pod1
kubectl get pods pod1
kubectl get po pod1

kubectl exec -it ["pod name"] -- /bin/bash | /bin/sh

kubectl logs ["pod name"]
kubectl config current-context
kubectl get replicaset
kubectl edit deployment deploy-name  // you will get live editor
```