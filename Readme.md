# Mongo-express Setup using Kubernetes

## commands to run.
## Install kubectl and minikube
```
brew install kubectl
brew install minikube   
```
## Create minikube with basic components such as configmap, serect, pod and service
```
minikube start
kubectl get pod
kubectl apply -f mongo-config.yaml
kubectl apply -f secret.yaml
kubectl apply -f mongo-app.yaml
kubectl apply -f web-app.yaml
kubectl get pod
kubectl get configmap
kubectl get secret
kubectl get svc
minikube ip
kubectl get node -o wide
```

## Assign the service to ip address and port 
```
minikube service webapp-service
```

## To delete the deployement and secret 
```
kubectl delete deployment --all
```
```
kubectl delete secret --all
```
