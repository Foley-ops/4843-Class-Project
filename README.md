# Docker and Kubernetes: A Scalable Personal Website

## CS 4843 – Project Group 20

| Name                 | Responsibilities          |
|----------------------|---------------------------|
| Nicholas Foley       | Docker/Cloud/Video        |
| Emmanuel Castellanos | Website/Report            |
| Rodrigo Nunez        | Website/Report            |
| Nicholas O’Connell   |                           |

## Overview
Deploying a containerized personal website that scales with high traffic using Kubernetes. Demonstrating the efficiency of Docker in this context.

## Goals
- Show Kubernetes' load balancing capabilities.
- Manage containerized applications effectively.
- Set up a Kubernetes cluster.
- Deploy a Docker containerized web application.
- Ensure the application scales to handle increased traffic.

## Software Tools
- Docker
- Kubernetes
- Git
- Google Cloud/AWS

# Deployment Process

docker build -t gcr.io/cloudcomputing-4843-g20/static-website:v1 .
docker push gcr.io/cloudcomputing-4843-g20/static-website:v1

kubectl apply -f deployment.yaml
kubectl apply -f service.yaml

kubectl get pods ; kubectl get service
