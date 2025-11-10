# kubectl basics
## Install kubectl
### Windows

```powershell
PS > winget install -e --id Kubernetes.kubectl
```
Restart the powershell console.

## Pods

### Show pods in default namespace

```bash
> kubectl get pods
```

To show some additional information
```bash
> kubectl get pods -o=wide
```

To show pod additional information
```bash
> kubectl describe pods/my_pod_name
```
[Check describe in the Kubernetes documentation](https://kubernetes.io/docs/reference/kubectl/generated/kubectl_describe/)

### Run pod using a yaml file

```bash
> kubectl create -f ./my_pod_defintion.yaml
```

### Delete a pod
Using pod name:
```bash
> kubectl delete pod the_pod_name_to_kill
```
