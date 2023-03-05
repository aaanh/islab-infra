# Inertial Sensing Lab - Platform Engineering

## Technologies

-   Docker (underlying)
-   Kubernetes (k8s)
-   Helm
-   Shell scripting

## Prerequisites

### kubectl

As the name suggests, `kubectl` is the command line interface for controlling `islab.ca` k8s cluster and resources.

Installation: <https://kubernetes.io/docs/tasks/tools/#kubectl>.

### helm

`helm` manages the packages and applications to be installed on the k8s cluster.

Installation: <https://helm.sh>

## Quick start

-   Switch context to production k8s cluster

```sh
export KUBECONFIG=/path/to/kubeconfig.yaml
```

-   Deploy

```
helm install --name <release-name> -f helmcharts/values.yaml requarks/wiki
```
