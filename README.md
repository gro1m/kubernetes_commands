# Commands

## Kubectl
```shell
kubectl get pods # gets pods in default namespace
kubectl get pods --namespace <namespace> # get pods in specific namespace <namespace>
kubectl get pods --namespace <namespace> -o yaml # get pods in specific namespace <namespace> in YAML format
kubectl describe pod <pod> --namespace <namespace> # get description of specified <pod> in specific namespace <namespace>
kubectl logs --follow <pod> --namespace <namespace> # print logs of pod <pod> in namespace <namespace>
```

## Helm Templating
Article:
- https://itnext.io/reference-other-values-in-helm-chart-values-file-19d44d9276c7
