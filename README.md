# argocd-kustomize

```
argocd login <ARGOCD_SERVER> --username admin --password <YOUR_PASSWORD>
```

```
argocd app create my-app \
  --repo <REPO_URL> \
  --path overlays/production \
  --dest-server https://kubernetes.default.svc \
  --dest-namespace default \
  --sync-policy automated \
  --upsert
```
