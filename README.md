# Kubernetes-deployment
Here's a simple Kubernetes deployment YAML file
It deploys an Nginx web server and includes a Service for external access. You can modify it to fit your needs.
Kubernetes Nginx Deployment

This repository contains a simple Kubernetes deployment configuration for deploying an Nginx web server. The deployment consists of:

A Deployment with three replicas of an Nginx container.

A Service of type LoadBalancer to expose the Nginx pods externally.

Prerequisites

Ensure you have the following installed before deploying:

Kubernetes CLI (kubectl)

A running Kubernetes cluster (Minikube, AKS, EKS, GKE, etc.)

Deployment

To deploy the Nginx server, run: kubectl apply -f deployment.yaml

Verifying Deployment:

Check if the pods are running: kubectl get pods

Check if the service is running: kubectl get svc nginx-service

If running in Minikube, access the service using: minikube service nginx-service

Cleanup: To remove the deployment and service, run: kubectl delete -f deployment.yaml


This project is licensed under the MIT License.