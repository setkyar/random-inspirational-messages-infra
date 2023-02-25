kubectl create namespace frontend

### Create deployment
```
kubectl apply -f deployment.yaml -n frontend
```

### Delete deployment
```
kubectl delete deployment frontend-deployment -n frontend
```

### Get pods in frontend specific namespace
kubectl get pods -n frontend

### Create frontend service
kubectl apply -f service.yaml -n frontend

### Get frontend services
kubectl get services -n frontend