# Day 2 Slide 9

```
Day2/2.Afternoon/1. HPA

kubectl apply -f php.yaml
kubectl get deployment php-apache 
kubectl get svc php-apache

```

# Day 2 slide 10

`
kubectl apply -f hpa.yaml
kubectl get hpa

`

# Day 2 slide 11


```
kubectl run -i --tty load-generator --rm --image=busybox:1.28 --restart=Never -- /bin/sh -c "while sleep 0.01; do wget -q -O- http://php-apache; done"

```

# Day 2 slide 12

`
kubectl get hpa http-app --watch
`

# Day 2 slide 13

```
kubectl get pod | grep php
```

# Day 2 slide 21

```
git clone https://github.com/kubernetes/autoscaler.git
cd autoscaler/vertical-pod-autoscaler
```

# Day 2 slide 22

```
./hack/vpa-up.sh

```

# Day 2 slide 23

```
kubectl get pods -n kube-system
```

# Day 2 slide 24

```
kubectl apply -f examples/hamster.yaml

```

# Day 2 slide 25

```
kubectl get vpa

```

# Day 2 slide 29

```
kubectl describe vpa hamster-vpa

```

# Day 2 slide 27

```
kubectl describe pod hamster-xxxx-t6xxxxdxv

```

# Day 2 slide 32

```
Day2/2.Afternoon/3. CA
kubectl apply -f php.yaml

```

# Day 2 slide 33

```
kubectl scale --replicas=10 deployment php
```

# Day 2 slide 35

```
kubectl describe configmap cluster-autoscaler-status -n kube-system
```

# Day 2 slide 37

```
kubectl get nodes
```

# Day 2 slide 38

```
kubectl get pod | grep php
```

# Day 2 slide 39

```
kubectl scale --replicas=1 deployment php 
```

# Day 2 slide 41

```
kubectl describe configmap cluster-autoscaler-status -n kube-system

```

# Day 2 slide 42

```
kubectl get nodes
```

# Day 2 slide 42

```
kubectl get nodes
```