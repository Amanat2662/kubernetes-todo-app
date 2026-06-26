# Kubernetes Todo App

A multi-tier Todo application deployed on Kubernetes.

## Architecture
- Frontend: Nginx
- Backend: Nginx (simulated)
- Database: MySQL 5.7

## Kubernetes Concepts Used
- Namespace
- Deployments & Services
- ConfigMap & Secrets
- Persistent Volume & PVC
- Ingress

## How to Run
1. Apply all manifests:
   kubectl apply -f todo-secret.yaml
   kubectl apply -f todo-configmap.yaml
   kubectl apply -f todo-pv.yaml
   kubectl apply -f todo-pvc.yaml
   kubectl apply -f todo-mysql.yaml
   kubectl apply -f todo-backend.yaml
   kubectl apply -f todo-frontend.yaml
   kubectl apply -f todo-ingress.yaml

2. Access the app:
   minikube service todo-frontend-service -n todo-app
