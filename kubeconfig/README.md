
# Disclaimer 

This Script has been tested working in 

- GKE Cluster
- Self Deployed Kubernetes Cluster

# Execute the following 

```
kubectl apply -f https://github.com/myawsm/ops/blob/main/kubeconfig/svc-deployer.yaml
bash https://github.com/myawsm/ops/blob/main/kubeconfig/gen-kubeconfig.yaml
```

- Create a Kubernetes service account named svc-deployer.
- Assign the cluster-admin role to the svc-deployer service account.
- Generate a kubeconfig file in the directory where the above commands are executed.

# Verification 

```
kubectl --kubeconfig kubeconfig get nodes
```