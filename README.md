# helm-charts
Helm repository of following charts:

* [k8s-deployment-restarter](https://github.com/kostiantyn-matsebora/k8s-deployment-restarter-chart) -  restarts kubernetes deployment resource by schedule.
* [storage-provisioner](https://github.com/kostiantyn-matsebora/storage-provisioner-chart) - provisioning of storage definition (PersistentVolumeClaim and PersistentVolume objects).
* [oauth2-proxy-oidc](https://github.com/kostiantyn-matsebora/oauth2-proxy-oidc-chart) - oauth2-proxy configured to use OIDC provider for user authentication.
* [coredns-custom](https://github.com/kostiantyn-matsebora/coredns-custom-chart) - CoreDNS custom/additional configuration.

## Usage

Add repository first:

```
helm repo add kostiantyn-matsebora https://kostiantyn-matsebora.github.io/helm-charts/
```

Install helm chart using your custom values (for instance storage-provisioner):
```
helm install kostiantyn-matsebora/storage-provisioner --values ./custom-values.yaml
```
