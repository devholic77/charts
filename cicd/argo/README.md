### mongodb
* github repo : https://github.com/argoproj/argo-helm/tree/master/charts/argo-cd
* values.yaml : https://github.com/argoproj/argo-helm/blob/master/charts/argo-cd/values.yaml

```sh
# repo 추가
> helm repo add argo https://argoproj.github.io/argo-helm

# 설치
> helm install argo argo/argo-cd --values=./values.yaml

# 삭제
> helm delete argo 
```
