# Api Local Setup

## Prerequisites

### Install
- Install Docker Desktop and enable Kubernetes in settings
- `scoop install kubectl`
- `scoop install helm`
- `scoop bucket add extras && scoop install skaffold`
- `scoop install terraform`

### Kubernetes (optional)
- [Set up dashboard](https://kubernetes.io/docs/tasks/access-application-cluster/web-ui-dashboard/)

## Getting Started

### Provision infrastructure
- cd to `~/deploy/k8s/terraform/local`
- `terraform init`
- `terraform apply`

### Deploy application
- cd to root
- `skaffold run -n pitch-api`

### Hosts
Add the following to your hosts file:
```
192.168.1.115 localhost.pitch-game.io
```