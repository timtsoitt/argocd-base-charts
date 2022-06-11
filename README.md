# argocd-base-charts

This repository is storing a nginx helm chart for demonstration purpose.

To transform a Github repository to Helm chart repository, run these commands.

```
cd releases
ls -d ../charts/* | xargs helm package 
helm repo index .
```

To use this Helm chart repository, run this command.

`helm repo add argocd-charts https://raw.githubusercontent.com/timtsoitt/argocd-base-charts/main/releases`