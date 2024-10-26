```
k create ns newrole
```
```
k create role ro-acc --namespace=newrole --verb=get,watch,list,update --resource=pod --dry-run=client -o yaml > ro-acc-08.yaml
```
- Apply the maniifest