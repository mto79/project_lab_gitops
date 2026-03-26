# project_lab GitOps

GitOps configuration for `project_lab` managed with **ARGOCD**.

## Environments


- `dev`

- `staging`

- `prod`


## Bootstrap


```bash
kubectl create namespace argocd
kubectl apply -n argocd -f bootstrap/argocd/install.yaml
kubectl apply -n argocd -f bootstrap/argocd/app-of-apps.yaml
```

