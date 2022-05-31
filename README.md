# k8s-demo
A demo for Kubernetes using mongoDB.

### start minikube with docker as a dirver
```
minikube start —driver docker 
```

### create config files
```
kubectl apply -f mongo-config.yaml 
kubectl apply -f mongo-secret.yaml 
kubectl apply -f mongo.yaml 
kubectl apply -f webapp.yaml 
```


### verify all components creation
```
kubectl get all
```


### get internal IP of the node
```
kubectl get node -o wide
```


### get the port of the service
```
kubectl get svc
```

you can now access the application externally on the nodeIP:svcPort

