# Commands

```shell
kubectl get pods # gets pods in default namespace
kubectl get pods --namespace <namespace> # get pods in specific namespace <namespace>
kubectl describe pod <pod> --namespace <namespace> # get description of specified <pod> in specific namespace <namespace>
kubectl logs --follow <pod> --namespace <namespace> # print logs of pod <pod> in namespace <namespace>
```
