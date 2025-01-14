
## helm Command list

```
helm repo add prometheus-community https://prometheus-community.github.io/helm-charts
helm repo update
helm search repo prometheus-community
helm show values prometheus-community/kube-prometheus-stack

helm show values prometheus-community/kube-prometheus-stack > values.yaml
helm install prometheus prometheus-community/kube-prometheus-stack
kubectl get statefulset
kubectl describe  statefulset prometheus-prometheus-kube-prometheus-prometheus 
kubectl describe  statefulset prometheus-prometheus-kube-prometheus-prometheus > prometheus.yaml

```