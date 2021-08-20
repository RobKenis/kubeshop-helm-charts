![Known Vulnerabilities](https://snyk.io/test/github/kubeshop/helm-charts/badge.svg)

# Kubeshop Helm Charts

This repo contains Helm Charts for Kubeshop projects and makes them available as a 
Helm Repository at https://kubeshop.github.io/helm-charts.

## Helm installation

[Helm](https://helm.sh) must be installed to use the charts.  Please refer to
Helm's [documentation](https://helm.sh/docs) to get started.

Once Helm has been set up correctly, add the repo as follows:

```sh
helm repo add kubtest-helm-charts https://kubeshop.github.io/helm-charts
```

If you had already added this repo earlier, run `helm repo update` to retrieve
the latest versions of the packages.  You can then run `helm search repo
kubtest-helm-charts` to see the charts.

## Kubtest Helm Charts

The following [Kubtest](https://github.com/kubeshop/kubtest/) Helm Charts are in this project
 
- `api-server`: the Kubtest API Server
- `kubtest-operator`: the Kubtest Operator
- `postman-executor`: the Postman Executor used for running Postman Collections
- `kubtest`: the main Kubtest chart - [Installation Instructions](https://kubeshop.github.io/kubtest/installing/#manual-kubtest-helm-charts-installation)

> Please note that the kubtest Helm chart will install all the needed charts. Including CRDs. It's an umbrella chart.

If you're interested to see what these Helm Charts install you can use [Monokle](https://github.com/kubeshop/monokle) to 
load and preview all of them:
- clone this repository 
- load the project folder into Monokle
- select and preview each of the Helm charts as described at [Working with Helm](https://kubeshop.github.io/monokle/helm/)