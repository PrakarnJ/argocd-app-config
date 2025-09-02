# ArgoCD Application Configuration

This repository stores the Kubernetes manifest files for the `myapp` application, managed by ArgoCD.

## Structure

- `application.yaml`: The ArgoCD Application resource definition. This points to the `dev` directory in this repository.
- `dev/`: Contains the Kubernetes manifests for the development environment.
  - `deployment.yaml`: Defines the deployment for `myapp`.
  - `service.yaml`: Defines the service to expose `myapp`.

## Usage

This repository is intended to be used with an ArgoCD instance. The `application.yaml` can be applied to your cluster to have ArgoCD manage the application.

```bash
kubectl apply -f application.yaml
```
