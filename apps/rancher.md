# Rancher

**Rancher**, the open-source multi-cluster orchestration platform, lets operations teams deploy, manage and secure enterprise **Kubernetes ([[kubernetes]])**.

Project Homepage: [Rancher Homepage](https://www.rancher.com/)

---

## [](https://github.com/ChristianLempa/cheat-sheets/blob/main/apps/rancher.md#remove-installation)Remove Installation

```
kubectl delete validatingwebhookconfiguration rancher.cattle.io
kubectl delete mutatingwebhookconfiguration rancher.cattle.io
```