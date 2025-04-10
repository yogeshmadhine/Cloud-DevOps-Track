# Day 1 - Docker

This folder contains the Docker implementation for the Sorting Visualizer project.

## Contents

- `Dockerfile`: Defines the environment and steps to build a Docker image for the application.
- `index.html`: Main HTML page for the sorting visualizer.
- `style.css`: Stylesheet for the visualizer UI.
- `README.md`: Documentation for the Docker setup.

## Usage

To build and run the Docker container:

```bash
docker build -t sorting-visualizer .
docker run -p 8080:80 sorting-visualizer

Then, open http://localhost:8080 in your browser to view the application.

# Day 2 - Kubernetes Deployment

This directory contains the Kubernetes setup for deploying the Sorting Visualizer application.

## Folder Structure

- `index.html` – Main HTML interface for the visualizer
- `style.css` – Styling for the UI
- `script.js` – Sorting logic and interactivity
- `deployment.yaml` – Kubernetes Deployment configuration
- `service.yaml` – Kubernetes Service to expose the deployment
- `README.md` – Documentation for Day 2

## Prerequisites

- A running Kubernetes cluster (Minikube or any other)
- `kubectl` command-line tool configured to interact with the cluster

## How to Deploy

1. Apply the deployment configuration:

   ```bash
   kubectl apply -f deployment.yaml
    This command will open the application in your default web browser.

Notes

    The deployment creates a pod running a simple static server to serve the sorting visualizer.

    The service exposes the pod on a NodePort, making it accessible from outside the cluster (in Minikube or other setups).
