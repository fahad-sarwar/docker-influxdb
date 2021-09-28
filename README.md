# docker-influxdb

https://kubernetes.io/docs/tasks/configure-pod-container/translate-compose-kubernetes/

To convert the docker-compose.yml file to files that you can use with kubectl, run kompose convert and then kubectl apply -f <output file>.
  
```
kompose convert
```

```
kubectl apply -f frontend-service.yaml,redis-master-service.yaml,redis-slave-service.yaml,frontend-deployment.yaml,
```
