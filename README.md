# Deployment configuration for Kubernetes local path provisioner 

![Deployment Status](https://argocd.vivaconagua.org/api/badge?name=k8s-local-path-provisioner&revision=true)

This repository consists of kubernetes manifests that deploy a [local-path-provisioner](https://github.com/rancher/local-path-provisioner) for Kubernetes on our cluster the way we want it to.

## Deployed configuration

Deployment configuration is mainly done from [config.json](./config.json) (see [reference](https://github.com/rancher/local-path-provisioner#configuration=)).
The only thing we do is to change the host path under which volumes are created to `/srv/k8s/local-path-provisioner`.
