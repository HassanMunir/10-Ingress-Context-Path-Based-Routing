# Steps to follow

/// Step-01: Deploy and Verify

```shell

### Step 01.01 Deploy Apps ###
kubectl apply -R -f kube-manifests/

### Step 01.02 List Pods ###
kubectl get pods

### Step 01.03 List Services ###
kubectl get svc

### Step 01.04 List Ingress ###
kubectl get ingress

### Step 01.05 Verify Ingress Controller Logs ###
kubectl get pods -n ingress-basic
kubectl logs -f <pod-name> -n ingress-basic
```

/// Step-02: Clean-Up Applications

```shell
### Step 02-01 Delete Apps
kubectl delete -f kube-manifests/

### Step 02-02 Delete Azure Disk created for Usermgnt Web App
Go to All Services -> Azure Disks -> Delete disk
```
