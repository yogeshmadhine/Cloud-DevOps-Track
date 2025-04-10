# Day 3 - AWS EKS Cluster Deployment

This folder contains documentation for deploying the Sorting Visualizer application using AWS Elastic Kubernetes Service (EKS).

## Contents

- EKS cluster creation using eksctl
- Docker image build and push to AWS ECR
- Kubernetes deployment and service
- Accessing the deployed app via LoadBalancer

## Requirements

- AWS CLI, eksctl, kubectl installed
- Docker installed and configured
- An AWS account with necessary permissions

## Steps Overview

1. Create an EKS cluster with `eksctl`
2. Build and push Docker image to Amazon ECR
3. Apply `deployment.yaml` and `service.yaml` using `kubectl`
4. Access the application using the external LoadBalancer IP
