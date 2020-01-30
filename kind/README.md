# A KIND with tekton playground

## Quick Information

- Istio - Work in progress (do not use)

## Requirements

- <https://taskfile.dev>
- envrc

## Installation

`task kind-install`

## Create cluster

`task create-cluster`

## Delete cluster

`task delete-cluster`

## Kubeconfig via envrc

`task kubeconfig`

## Monitoring quick start

```bash
task kind-install
task tools-helm
task create-cluster
#Envrc required to work \/
task kubeconfig
task deploy-monitoring-stack
```

### Grafana Dashboards

```bash
task port-forward-grafana
# Open in browser http://localhost:9097
```

