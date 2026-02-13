## Apply All Kubernetes Manifests

Apply all YAML files in the current directory:

```bash
kubectl apply -f .
```

## Verify Deployment

Get the IP address of the current node

```bash
kubectl get deployments
```

```bash
kubectl get nodes -o wide 
```

## Access the Voting App

The vote service will be accessible through the following URL:

```
http://<ip_address_of_the_node>:31000
```

## Scale the Voting App Deployment

This command updates the desired replica count of the `vote` deployment to 5. 

```bash
kubectl scale deployment vote --replicas=5
```