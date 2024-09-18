# helm-charts
Helm repository of the following charts:

* [Deployment restarter](https://github.com/kostiantyn-matsebora/helm-k8s-deployment-restarter) -  restarts kubernetes deployment resource by schedule.
* [Storage provisioner](https://github.com/kostiantyn-matsebora/helm-storage-provisioner) - provisioning of storage definition (PersistentVolumeClaim and PersistentVolume objects).
* [oauth2-proxy OIDC](https://github.com/kostiantyn-matsebora/helm-oauth2-proxy-oidc) - oauth2-proxy configured to use OIDC provider for user authentication.
* [Custom CoreDNS](https://github.com/kostiantyn-matsebora/helm-coredns-custom) - CoreDNS custom/additional configuration.
* [Generic application](https://github.com/kostiantyn-matsebora/helm-generic-application) - Generic application with features.
* 
## Usage

Add repository first:

```bash
helm repo add kostiantyn-matsebora https://kostiantyn-matsebora.github.io/helm-charts/
```

Install helm chart using your custom values (for instance storage-provisioner):
```
helm install kostiantyn-matsebora/storage-provisioner --values ./custom-values.yaml
```
