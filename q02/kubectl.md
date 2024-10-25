```
k create deployment my-project --replicas=1 --image=nginx:1.16 --dry-run=client -o yaml > my-proj-02.yaml
```
- Apply the manifest
```
k get deployments.apps my-project -o wide
```
```
k set image deployments my-project nginx=nginx:1.17
```
```
k get deployments.apps my-project -o wide
```