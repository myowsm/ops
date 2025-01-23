
# Disclaimer 

This Script has been tested working in 

- GKE Cluster
- Self Deployed Kubernetes Cluster

# Execute the following 

```
kubectl apply -f https://raw.githubusercontent.com/myowsm/ops/refs/heads/main/kubeconfig/svc-deployer.yaml
curl -sL https://raw.githubusercontent.com/myowsm/ops/refs/heads/main/kubeconfig/gen-kubeconfig.sh | bash
```

- Create a Kubernetes service account named svc-deployer.
- Assign the cluster-admin role to the svc-deployer service account.
- Generate a kubeconfig file in the directory where the above commands are executed.

# Verification 

```
kubectl --kubeconfig kubeconfig get nodes
```