# k8s-infrastructure-iac: Flask on AWS EKS

A cloud-native Python Flask application containerized with Docker and orchestrated using Kubernetes on AWS Elastic Kubernetes Service (EKS).

![Python](https://img.shields.io/badge/Python-3.9-blue)
![Docker](https://img.shields.io/badge/Docker-Container-blue)
![Kubernetes](https://img.shields.io/badge/Kubernetes-AWS%20EKS-orange)

##  Project Overview
This project demonstrates a complete DevOps workflow for deploying a microservice:
1.  **Application:** A Python Flask web application.
2.  **Containerization:** Dockerized for portability.
3.  **Orchestration:** Deployed on a 2-node AWS EKS Cluster.
4.  **Networking:** Exposed to the internet via an AWS Classic Load Balancer (CLB).

## Technologies Used
* **Language:** Python 3 (Flask)
* **Containerization:** Docker
* **Orchestration:** Kubernetes (K8s)
* **Cloud Provider:** AWS (EKS, EC2, ELB)
* **Infrastructure Tools:** `eksctl`, `kubectl`

## How to Run

### 1. Prerequisites
* AWS CLI configured
* Docker installed
* `kubectl` and `eksctl` installed

### 2. Build the Docker Image
```bash
docker build -t your-dockerhub-username/musical-spoon:latest .
docker push your-dockerhub-username/musical-spoon:latest
