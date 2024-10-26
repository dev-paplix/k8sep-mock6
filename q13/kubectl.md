```
k create deployment book --image=httpd:bookworm --dry-run=client -o yaml > book-14.yaml
```
- Apply the manifest

```
k expose deployment book --name=<>??????
```