# Kubectl Demo

## Nginx 🧩

- [nginx.yaml](./nginx/nginx.yaml)

## Minecraft 🧱

- [minecraft-bedrock.yaml](./minecraft-bedrock/minecraft-bedrock.yaml)

## Portainer

https://node1:30443

- The NodePort exposes it on ports 30443 (HTTPS) and 30000 (HTTP) on all cluster nodes.
- Data is stored in a PVC (portainer-data) so it persists across restarts

To deploy:
1. Putty to the master node 
2. Clone https://github.com/carlpaton/kubectl-demo
3. cd `portainer`
4. Run kubectl deployment

```
kubectl apply -f portainer.yaml
kubectl get pods -n portainer
```

- [portainer.yaml](./portainer/portainer.yaml)