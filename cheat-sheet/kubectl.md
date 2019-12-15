# Cheat Sheet
## Viewing Resource Information
---
### **Nodes**

```bash
kubectl get no
kubectl get no -o wide
kubectl describe no
kubectl get no -o yaml
kubectl get node --selector=[label_name]
kubectl get nodes -o jsonpath='{.items[*].status.address[?(@.type=="ExternalIP")].address}'
kubectl top [node_name]
```

### **Pods**

```bash
kubectl get po
kubectl get po -o wide
kubectl describe po
kubectl get po --show-labels
kubectl get po -l app=nginx
kubectl get po -o yaml
kubectl get pod [pod_name] -o yaml --export
kubectl get pod [pod_name] -o yaml --export > nameoffile.yaml
kubectl get pods --filed-selector status.phase=Running
```

### **Namespaces**
```bash
kubectl get ns
kubectl get ns -o yaml
kubectl describe ns
```



