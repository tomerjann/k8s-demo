# Start minikube

minikube start --vm-driver=hyperkit
minikube status

# Deploy application

kubectl apply -f mongo-config.yaml

kubectl apply -f mongo-secret.yaml

kubectl apply -f mongo.yaml

kubectl apply -f webapp.yaml

kubectl apply -f .

# Common commands

kubectl get all

kubectl get configmap

kubectl get secret

kubectl get pod

kubectl get svc -o wide

# Get minikube node's ip address

minikube ip

# Open minikube ip with nodePort 30100

192.168.64.2:30100

# Stop minikube

minikube stop
