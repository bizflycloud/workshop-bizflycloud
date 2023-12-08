# Day 1 slide 6
`
git clone https://github.com/bizflycloud/workshop-bizflycloud.git
`

Day1/1.Morning/1.Docker/app.py

Day1/1.Morning/1.Docker/Dockerfile

# Day 1 slide 7

`docker build -t python-helloword .`

# Day 1 slide 14 -> 16

```
sudo docker login -u BIZFLY -p <token> cr-hn-1.bizflycloud.vn

docker tag python-helloword:latest cr-hn-1.bizflycloud.vn/cecd854937c8421b81d1d73789acad52/python-helloword:latest

sudo docker push cr-hn-1.bizflycloud.vn/cecd854937c8421b81d1d73789acad52/python-helloword:latest
```

# Day 1 slide 18


```
sudo docker run cr-hn-1.bizflycloud.vn/cecd854937c8421b81d1d73789acad52/python-helloword:latest
```

# Day 1 slide 22

```
Day1/1.Morning/2.Kubernetes/deployment.yaml
kubectl apply -f deployment.yaml
```

# Day 1 slide 25-26

```
kubectl get pod

kubectl get pod -A

kubectl describe pod <pod-name>
```

# Day 1 slide 29->30

```
kubectl get replicasets

kubectl get deployment
``