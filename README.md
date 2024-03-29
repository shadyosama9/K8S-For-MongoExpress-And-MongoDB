# MongoDB and MongoDB Express Cluster Deployment

This repository contains Kubernetes YAML files to deploy a MongoDB cluster and MongoDB Express for easy management.

## Prerequisites

- [Minikube](https://minikube.sigs.k8s.io/docs/start/)
- [kubectl](https://kubernetes.io/docs/tasks/tools/install-kubectl/)

## Deployment

1. **Start Minikube:**
   ```sh
   minikube start

2. **Deploy MongoDB:**
     ```sh
    kubectl apply -f mongodb-deploy.yml

3. **Deploy MongoDB Express:**
      ```sh
   kubectl apply -f mongoexp-deploy.yml

4. **Attach an external IP for the MongoDB Express service:**
      ```sh
    minikube service mongoexpress-service
