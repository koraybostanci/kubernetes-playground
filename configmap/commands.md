# ConfigMap

- Create a configmap from literals

```sh
kubectl create configmap myconfigs \
--from-literal=background=white \
--from-literal=fontsize=14
```

- Create a configmap from file

```sh
kubectl create configmap myconfigs \
--from-file=configs.json
```

- Print environment variables of a pod

```sh
kubectl exec <pod-name> -n <namespace> -- printenv
```

- List or display a mounted path in the pod

```sh
kubectl exec <pod-name> -n <namespace> -- ls /var/config
kubectl exec <pod-name> -n <namespace> -- cat /var/config/settings
```
