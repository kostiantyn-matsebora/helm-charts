# Helm charts repository 

[![Artifact Hub](https://img.shields.io/endpoint?url=https://artifacthub.io/badge/repository/kostiantyn-matsebora-helm-charts)](https://artifacthub.io/packages/search?repo=kostiantyn-matsebora-helm-charts)

It contains the following charts:

* [Deployment restarter](https://github.com/kostiantyn-matsebora/helm-k8s-deployment-restarter) -  restarts kubernetes deployment resource by schedule.
* [Storage provisioner](https://github.com/kostiantyn-matsebora/helm-storage-provisioner) - provisioning of storage definition (PersistentVolumeClaim and PersistentVolume objects).
* [Simple oauth2-proxy](https://github.com/kostiantyn-matsebora/helm-simple-oauth2-proxy) - deploying and configuring oauth2-proxy provides a way to configure OIDC provider as any other OAuth2 provider supported by application..
* [Custom CoreDNS](https://github.com/kostiantyn-matsebora/helm-coredns-custom) - CoreDNS custom/additional configuration.
* [Any application](https://github.com/kostiantyn-matsebora/helm-generic-application) - Generic application with features.

## Usage

Add repository first:

```bash
helm repo add kostiantyn-matsebora https://kostiantyn-matsebora.github.io/helm-charts/
```

Install/upgrade helm chart using your custom values (for instance storage-provisioner):
```bash
# Storage provisioner
helm upgrade deployment-restarter kostiantyn-matsebora/storage-provisioner --install --values ./custom-values.yaml

# Deployment restarter
helm upgrade deployment-restarter kostiantyn-matsebora/k8s-deployment-restarter --install --values ./custom-values.yaml

# Simple oauth2-proxy
helm upgrade oauth2-proxy kostiantyn-matsebora/simple-oauth2-proxy --install --values ./custom-values.yaml

# Custom CoreDNS
helm upgrade coredns-custom kostiantyn-matsebora/coredns-custom --install --values ./custom-values.yaml

# Any application
helm upgrade myapp kostiantyn-matsebora/application --install --values ./custom-values.yaml
```
