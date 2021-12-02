# Service

- Create a service from a deployment

```sh
kubectl expose deploy nginx \
--type=ClusterIP \
--name=nginx \
--port='8080' \
--target-port='80'
```

- Fetch endpoints created per created services

```sh
kubectl get endpoints -o wide
```
