# Dodo Payments – DevSecOps Assignment

## Candidate

Lingaraj S H

## Overview

This repository contains my solution for the Dodo Payments DevSecOps Practical Assignment.

### Task 1 – Secure Kubernetes Deployment ✅

The Ledger API has been deployed securely on a local Kubernetes cluster (Minikube).

## Technologies Used

- Ubuntu 24.04
- Docker
- Kubernetes
- Minikube
- kubectl

## Implemented

- Kubernetes Namespace
- ConfigMap
- Secret
- ServiceAccount
- RBAC (Role & RoleBinding)
- Deployment (2 replicas)
- ClusterIP Service
- NGINX Ingress

## Verification

Application verified using:

```bash
kubectl get all -n payments
kubectl get ingress -n payments
curl http://localhost:9090/health
```

Browser:

```
http://ledger.local/health
```

Response:

```json
{
  "status": "ok"
}
```

## Repository Structure

```
app/
deploy/
task-1-secure-kubernetes/
images devsecops/
README.md
```
## Deployment Screenshots

The following screenshots demonstrate the successful deployment, verification, and secure configuration of the Ledger API on Kubernetes.

### 1. Namespace and Kubernetes Resources
![Namespace and Resources](images%20devsecops/Screenshot%20from%202026-07-13%2006-05-33.png)

### 2. Deployment Verification
![Deployment](images%20devsecops/Screenshot%20from%202026-07-13%2006-06-19.png)

### 3. Services and Pods
![Services](images%20devsecops/Screenshot%20from%202026-07-13%2006-07-00.png)

### 4. Ingress Configuration
![Ingress](images%20devsecops/Screenshot%20from%202026-07-13%2006-07-46.png)

### 5. Health Check
![Health Check](images%20devsecops/Screenshot%20from%202026-07-13%2006-10-14.png)

### 6. Browser Verification
![Browser](images%20devsecops/Screenshot%20from%202026-07-13%2006-10-40.png)

### 7. Final Deployment Status
![Status](images%20devsecops/Screenshot%20from%202026-07-13%2006-11-33.png)

## Author

Lingaraj S H
