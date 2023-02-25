### Create deployment
```
kubectl apply -f deployment.yaml -n backend
```

### Delete deployment
```
kubectl delete deployment backend-deployment -n backend
```

### Get pods in backend specific namespace
kubectl get pods -n backend

### Create backend service
kubectl apply -f service.yaml -n backend

### Get backend services
kubectl get services -n backend