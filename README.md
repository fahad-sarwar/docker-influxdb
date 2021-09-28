# docker-influxdb

https://kubernetes.io/docs/tasks/configure-pod-container/translate-compose-kubernetes/

To convert the docker-compose.yml file to files that you can use with kubectl, run kompose convert and then kubectl apply -f <output file>.
  
```
kompose convert
```

```
kubectl apply -f frontend-service.yaml,redis-master-service.yaml,redis-slave-service.yaml,frontend-deployment.yaml,
```

## Running locally
1. Check that it worked by running the following:

```
kubectl port-forward service/grafana 3000:3000
```

2. Navigate to ```localhost:3000``` in your browser. You should see a Grafana login page.

3. Use admin for both the username and password to login.
