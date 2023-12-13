# Day 2 Slide 8

```
https://helm.sh/docs/intro/install/

curl -fsSL -o get_helm.sh https://raw.githubusercontent.com/helm/helm/main/scripts/get-helm-3
chmod 700 get_helm.sh
./get_helm.sh
```

# Day 2 slide 9

`
helm repo add grafana https://grafana.github.io/helm-charts
helm repo update
helm upgrade --install loki --create-namespace --namespace=loki-stack grafana/loki-stack --set grafana.enabled=true
`

# Day 2 slide 10


```
kubectl get pod -n loki-stack
```

# Day 2 slide 11

`
kubectl get service -n loki-stack
`

# Day 2 slide 12

```
kubectl port-forward --namespace loki-stack service/loki-grafana 3000:80 --address '0.0.0.0'
```

# Day 2 slide 13

```
http://localhost:3000/login
```

# Day 2 slide 14

```
kubectl get secret --namespace loki-stack loki-grafana -o jsonpath="{.data.admin-password}" | base64 --decode ; echo
```

# Day 2 slide 21

```
kubectl top pod

kubectl apply -f https://github.com/kubernetes-sigs/metrics-server/releases/latest/download/components.yaml

kubectl top pod
```

# Day 2 slide 26

```
helm repo add prometheus-community https://prometheus-community.github.io/helm-charts
helm repo update

```

# Day 2 slide 28

```
helm install prometheus-stack --namespace prometheus-stack --create-namespace prometheus-community/kube-prometheus-stack -f values.yaml

```

# Day 2 slide 29

```
kubectl get pod -n prometheus-stack
kubectl get svc -n prometheus-stack
```

# Day 2 slide 31

```
kubectl get svc -A | grep prometheus-stack-kube-prom-prometheus
```