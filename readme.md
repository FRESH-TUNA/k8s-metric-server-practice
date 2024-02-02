## README.md

```
kubectl -n kube-system edit deployment metrics-server


spec:
   containers:
   - args:
 	- --cert-dir=/tmp
 	- --secure-port=4443
 	- --kubelet-insecure-tls  	#1 lines 추가


# metric checks
kubectl top pods --all-namespaces
kubectl top nodes
```
