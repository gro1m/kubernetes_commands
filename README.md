# Commands

## Kubectl

| Command | Description   |
|---|---|
| `kubectl config get-contexts` | get contexts/environments |
| `kubectl config set-cluster <env-name> --server=<server-adress>` | set Kubernetes Cluster |
| `kubectl config set-context <env-name> --cluster=<cluster-name> --user=<username>` | set Kubernetes context/environment |
| `kubectl get pods` | gets pods in default namespace |
| `kubectl --namespace <namespace> get pods` | get pods in specific namespace `<namespace>` |
| `kubectl --namespace <namespace> get pods -o yaml` |  get YAML Specs for pods in specific namespace `<namespace>` in YAML format | 
| `kubectl --namespace <namespace> get pod <pod-name> -o yaml`  |  get YAML Specs for pod with specific name <pod-name> in specific namespace <namespace> in YAML format | 
| `kubectl --namespace <namespace> describe pod <pod-name>`  |  get description of pod specified via name <pod-name> in specific namespace `<namespace>` | 
| `kubectl --namespace <namespace> logs <pod-name>` | print logs of pod <pod-name> in specific namespace `<namespace>` |
| `kubectl --namespace <namespace> logs --follow <pod-name>` | print logs of pod <pod-name> in specific namespace `<namespace>` |
| `kubectl --namespace <namespace> get events <pod-name>` | get events of pod <pod-name> in specific namespace `<namespace>` |
| `kubectl --namespace <namespace> get events <pod-name> -p` | get events of previous pod <pod-name> (e.g. after a restart) |
| `kubectl --namespace <namespace> get deploy` | Get Deployments for specific namespace `<namespace>` |
| `kubectl --namespace dmkdm-t edit deploy <deployment name>` | Edit Deployment to Change Specs and have a new Pod to test with. Use the `get deploy` command avove to receive deployment name |

## Helm
| Command | Description   |
|---|---|
| `helm repo add <name> <chart-http-address>` | add chart with name `<name>` from URL `<chart-http-address>` |
| `helm template . --debug -f <values.yaml file>` | debug `values.yaml` file |
| `helm list -n <namespace>` | list charts in namespace `<namespace>`|


### Templating
Article:
- https://itnext.io/reference-other-values-in-helm-chart-values-file-19d44d9276c7
