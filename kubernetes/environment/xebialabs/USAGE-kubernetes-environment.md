### Prerequisites

To apply the files generated by this blueprint, execute the following command:

```
$ xl apply -f xebialabs/kubernetes-environment.yaml
```

Applying this XL YAML file will create:
* a `k8s.Master` infrastructure CI for your Kubernetes cluster,
* a `k8s.Namespace` for the namespace you specified, and
* an `udm.Environment` that refers to that `k8s.Namespace`.

Instantiate and apply the companion `kubernetes/application` blueprint to create an application that can be deployed to this environment.