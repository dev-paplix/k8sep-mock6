```
k run pod-multi --image=nginx --dry-run=client -o yaml > pod-multi-04.yaml
```

Edit the manifest
```
apiVersion: v1
kind: Pod
metadata:
  creationTimestamp: null
  labels:
    run: pod-multi
  name: pod-multi
spec:
  containers:
  - name: container1
    image: nginx
  - name: container2
    image: busybox
    command: ['sh', '-c', 'sleep 4800']
  dnsPolicy: ClusterFirst
  restartPolicy: Always
status: {}

```