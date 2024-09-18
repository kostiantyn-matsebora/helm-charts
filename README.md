# helm-charts
Helm repository of the following charts:

* [Deployment restarter](https://github.com/kostiantyn-matsebora/helm-k8s-deployment-restarter) -  restarts kubernetes deployment resource by schedule.
* [Storage provisioner](https://github.com/kostiantyn-matsebora/helm-storage-provisioner) - provisioning of storage definition (PersistentVolumeClaim and PersistentVolume objects).
* [oauth2-proxy OIDC](https://github.com/kostiantyn-matsebora/helm-oauth2-proxy-oidc) - oauth2-proxy configured to use OIDC provider for user authentication.
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

# oauth2-proxy OIDC
helm upgrade oauth2-proxy kostiantyn-matsebora/oauth2-proxy-oidc --install --values ./custom-values.yaml

# Custom CoreDNS
helm upgrade coredns-custom kostiantyn-matsebora/coredns-custom --install --values ./custom-values.yaml

# Any application
helm upgrade myapp kostiantyn-matsebora/application --install --values ./custom-values.yaml
```
