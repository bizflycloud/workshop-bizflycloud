# Day 1 Slide 6

`
git clone https://github.com/bizflycloud/workshop-bizflycloud.git
`

# Day 1 slide 7

`
Day1/2.Afternoon/wordpress/wordpress-nosql.yml
kubectl apply -f wordpress/wordpress-nosql.yml
`

# Day 1 slide 8


`
Day1/2.Afternoon/wordpress/wordpress-svc.yml
kubectl apply -f wordpress/wordpress-svc.yml
`

# Day 1 slide 13

`
Day1/2.Afternoon/mysql/mysql-pvc.yml
kubectl apply -f mysql/mysql-pvc.yml

Day1/2.Afternoon/mysql/mysql-secret.yaml
kubectl apply -f mysql/mysql-secret.yaml
`

# Day 1 slide 14

```
Day1/2.Afternoon/mysql/mysql-stateful.yml
kubectl apply -f mysql/mysql-stateful.yml

Day1/2.Afternoon/mysql/mysql-pvc.yml
kubectl apply -f mysql/mysql-pvc.yml
```

# Day 1 slide 15

```
kubectl get pod

kubectl get pvc

kubectl get pv
```

# Day 1 slide 17

```
Day1/2.Afternoon/mysql/mysql-svc.yml
kubectl apply -f mysql/mysql-svc.yml
```

# Day 1 slide 18

```
kubectl get svc
```

# DAy 1 slide 19

```
Day1/2.Afternoon/wordpress/wordpress-sql.yml
kubectl apply -f wordpress/wordpress-sql.yml

```

# Day 1 slide 24

```
kubectl apply -f https://raw.githubusercontent.com/kubernetes/ingress-nginx/controller-v1.8.2/deploy/static/provider/cloud/deploy.yaml
```

# Day 1 slide 26

```
kubectl get pod -n ingress-nginx

kubectl get svc -n ingress-nginx
```

# ay 1 slide 28

```
Day1/2.Afternoon/externaldns/externaldns.yaml

kubectl apply -f externaldns/externaldns.yaml
```

# Day 1 slide 33

```
kubectl apply -f https://github.com/cert-manager/cert-manager/releases/download/v1.13.2/cert-manager.yaml

```

# Day 1 slide 35

```
kubectl get pod -n cert-manager
```

# Day 1 slide 37

```
Day1/2.Afternoon/cert-manager/clusterissuer.yaml

kubectl apply -f cert-manager/clusterissuer.yaml
```

# Day 1 slide 38

```
Day1/2.Afternoon/cert-manager/ingress_tls.yaml

kubectl apply -f cert-manager/ingress_tls.yaml
```