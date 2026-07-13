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
README.md
```

## Author

Lingaraj S H
