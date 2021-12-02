# Secret

- Check details of the secret object

```sh
kubectl explain secret
```

- Create a secret from literals

```sh
kubectl create secret generic mysecret \
--from-literal=username=user1 \
--from-literal=password=password1
```

- Create a secret from file

```sh
kubectl create secret generic mysecret \
--from-file=config.json
```

- Print environment variables of a pod

```sh
kubectl exec <pod-name> -n <namespace> -- printenv
```
