```
k create deployment myproject --image=nginx:1.16

k set image deployment myproject nginx=nginx.1.17 --record

k rollout status deployment myproject

k rollout history deployment myproject
```