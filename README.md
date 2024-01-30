# Helm Charts

Add a new chart to this repository:

```sh
# Package the Helm chart and add the created .tgz file to this repository:
helm package my-chart
# Update the index.yaml file.
helm repo index helm-charts/ --url https://ricoberger.github.io/helm-charts/
```

Add this Helm repository:

```sh
helm repo add ricoberger https://ricoberger.github.io/helm-charts
helm repo list
```

Update and show charts:

```sh
helm repo update
helm search repo -l ricoberger/
```
