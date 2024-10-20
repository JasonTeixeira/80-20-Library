# Kubernetes: 80/20 Essential Command Library

## Overview
This section contains the essential Kubernetes commands to help you manage clusters, deployments, services, and security policies efficiently. The commands here adhere to the **80/20 rule**, meaning mastering these will cover 80% of your daily tasks and prepare you for both **CKA and CKS certifications**.

---

## 1. Cluster Management Commands
- `kubectl get nodes` – List nodes in the cluster.
- `kubectl describe nodes` – Show detailed info about a node.
- `kubectl drain <node>` – Safely evict pods from a node.
- `kubectl uncordon <node>` – Mark a node as schedulable again.
- `kubectl delete node <node>` – Remove a node from the cluster.

---

## 2. Deployments and Scaling
- `kubectl create deployment <name> --image=<image>` – Create a new deployment.
- `kubectl get deployments` – List all deployments.
- `kubectl rollout status deployment/<name>` – Monitor deployment rollout status.
- `kubectl scale deployment <name> --replicas=<number>` – Scale a deployment.
- `kubectl delete deployment <name>` – Delete a deployment.

---

## 3. Networking and Services
- `kubectl get services` – List all services in the cluster.
- `kubectl describe svc <service-name>` – Show details about a service.
- `kubectl expose deployment <name> --port=<port>` – Expose a deployment as a service.
- `kubectl get ingress` – List all ingress resources.
- `kubectl apply -f ingress.yaml` – Create/update ingress from YAML.

---

## 4. Troubleshooting and Logs
- `kubectl logs <pod-name>` – View logs for a pod.
- `kubectl describe pod <pod-name>` – Show detailed info about a pod.
- `kubectl exec -it <pod-name> -- /bin/bash` – Open a shell in a running pod.
- `kubectl get events` – List cluster events for troubleshooting.
- `kubectl top nodes` – Show CPU and memory usage of nodes.

---

## 5. Security and RBAC
- `kubectl create role <role-name> --verb=get --resource=pods` – Create a role.
- `kubectl create rolebinding <binding-name> --role=<role-name> --user=<username>` – Bind a role to a user.
- `kubectl auth can-i <verb> <resource>` – Check if a user can perform an action.
- `kubectl create secret generic <name> --from-literal=key=value` – Create a secret.
- `kubectl apply -f pod-security-policy.yaml` – Apply a security policy.

---

## 6. ConfigMaps and Secrets Management
- `kubectl create configmap <name> --from-literal=key=value` – Create a ConfigMap.
- `kubectl get configmaps` – List all ConfigMaps.
- `kubectl describe configmap <name>` – Show details of a ConfigMap.
- `kubectl delete configmap <name>` – Delete a ConfigMap.

---

## 7. Advanced Commands
- `kubectl get all -n <namespace>` – List all resources in a namespace.
- `kubectl rollout undo deployment/<name>` – Roll back a deployment.
- `kubectl set image deployment/<name> <container>=<new-image>` – Update a container image.
- `kubectl port-forward <pod-name> <local-port>:<remote-port>` – Forward a port from a pod.
- `kubectl label nodes <node> <key>=<value>` – Label a node.

---

## Conclusion
Mastering these 40 commands will significantly enhance your proficiency in Kubernetes, ensuring you're ready for both real-world tasks and the **CKA/CKS certifications**. Keep practicing by setting up clusters and applying these commands in live scenarios to build muscle memory.



