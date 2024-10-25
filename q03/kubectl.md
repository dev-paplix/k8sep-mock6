```
k create deployment my-deployment --image=nginx --replicas=3 --dry-run=client -o yaml > my-dpl-03.yaml
```
- Edit the manifest and add `restartPolicy: Always` if I'm not mistaken