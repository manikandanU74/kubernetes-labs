# kubernetes-labs
This repo contains Kubernetes demo labs and practicals as part of my DevOps learning journey
# Kubernetes Labs - DevOps Learning

This repository contains hands-on labs and practice demos for Kubernetes as part of my DevOps upskilling journey.

---

## 📌 Lab 1 - Create a Simple Pod

### 📝 Objective
Create a simple NGINX pod using YAML and verify it is running.

### 📂 Files Included
- `nginx-pod.yaml` – YAML definition for NGINX pod

### 💡 Steps Performed

1. Wrote a pod YAML file
2. Applied it using `kubectl apply`
3. Verified pod status and logs

### 🧪 YAML Code

```yaml
apiVersion: v1
kind: Pod
metadata:
  name: nginx-pod
spec:
  containers:
  - name: nginx-container
    image: nginx
    ports:
    - containerPort: 80
