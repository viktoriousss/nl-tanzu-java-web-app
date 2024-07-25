# nl-tanzu-java-web-app

This is a sample of a Java Spring app that works with Tilt and the Tanzu Application Platform.

The app can also be deployed to Tanzu Platform for Kubernetes, in this case the Tilt requirements is dropped. For Tanzu Platform you would need a tanzu.yml file in the root of the project, and additional configuration files in .tanzu/config.

## Dependencies (for TAP)
1. [kubectl CLI](https://kubernetes.io/docs/tasks/tools/)
1. [Tilt version >= v0.23.2](https://docs.tilt.dev/install.html)
1. Tanzu CLI and the apps plugin v0.2.0 which are provided as part of [Tanzu Application Platform](https://network.tanzu.vmware.com/products/tanzu-application-platform)
1. A cluster with Tanzu Application Platform, and the "Default Supply Chain", plus its dependencies. This supply chains is part of [Tanzu Application Platform](https://network.tanzu.vmware.com/products/tanzu-application-platform).

## Deploy the app to Tanzu Platform for Kubernetes

Just run 

```
tanzu deploy -y
```