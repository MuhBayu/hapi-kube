# hapi-kube

## Build Image
```bash
$ docker build -t muhbayu/hapi-kube:latest .
```

## Push Image
```bash
$ docker push muhbayu/hapi-kube:latest
```

## Apply Kube
```bash
$ kubectl apply -f ./kube-template/hapi-app.yaml
```

## Get All (pods,deployments,services,replicasets)
```bash
$ kubectl get all
```

## Testing internal kubernetes cluster to your localhost
```bash
$ kubectl port-forward service/hapi-kube 3000:3000
```
Open: http://localhost:3000