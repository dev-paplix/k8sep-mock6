```
k run web-pod --image=busybox --pod-running-timeout=3200s --dry-run=client -o yaml > pod-01.yaml
```
- Apply the manifest