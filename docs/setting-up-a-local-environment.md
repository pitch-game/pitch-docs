# Setting up a Local Environment

## API

### Prerequisites

#### Install
- `scoop install https://raw.githubusercontent.com/Ash258/scoop-Ash258/master/bucket/docker.json`
- `scoop install kubectl`
- `scoop install helm`
- `scoop install skaffold`
- `scoop install terraform`

#### Docker desktop
- Enable Kubernetes

#### Kubernetes (optional)
- [Set up dashboard](https://kubernetes.io/docs/tasks/access-application-cluster/web-ui-dashboard/)

### Getting Started

#### Provision infrastructure
- cd to `~/deploy/k8s/terraform/local`
- `terraform init`
- `terraform apply`

#### Deploy application
- cd to root
- `skaffold run -n pitch-api`

#### Hosts
Add the following to your hosts file:
```
192.168.1.115 localhost.pitch-game.io
```

## Frontend

