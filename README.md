# A KIND with tekton playground

## Quick Information

- Simple stack with monitoring/logging

## Requirements

- [Docker](https://www.docker.com/)
- [Docker-compose](https://docs.docker.com/compose/)
- [Task](https://taskfile.dev)
- [envrc](https://direnv.net/)

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
task kubernetes-install
task kind-install
task tools-helm
task create-cluster
#Envrc required to work
task kubeconfig
task deploy-ingress
task deploy-monitoring-stack
```

### Grafana Dashboards

```bash
task port-forward-grafana
# Open in browser http://localhost:3000
# credentials admin/12tsh3
```


### Prometheus Dashboards

```bash
task port-forward-prometheus
# Open in browser http://localhost:9090
```

