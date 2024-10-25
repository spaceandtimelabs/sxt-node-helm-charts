# Sxt Node Chart Repo

sxt-node helm chart repository

For installation on Kubernetes we have created a helm chart sxt-node-chart. Adding Helm repository with following command:

```helm repo add sxt-charts https://spaceandtimelabs.github.io/sxt-node-chart-repo```

Once the Helm configuration is done, we can now run the following command with proper KUBECONFIG to install the chart:

```helm upgrade --install sxt-testnet-validator sxt-charts/sxt-node-chart --version=0.3.4 -n sxt-testnet --create-namespace -f ./values.yaml --dependency-update```




