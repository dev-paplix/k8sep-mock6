```
k run nginx-jaud00401 --image=nginx --dry-run=client -o yaml > pod-07.yaml
```

Edit the manifest
```
apiVersion: v1
kind: Pod
metadata:
  creationTimestamp: null
  labels:
    run: nginx-jaud00401
  name: nginx-jaud00401
spec:
  containers:
  - image: nginx
    name: nginx-jaud00401
    resources: {}
  nodeSelector:
    disktype: ssd
  dnsPolicy: ClusterFirst
  restartPolicy: Always
status: {}
```