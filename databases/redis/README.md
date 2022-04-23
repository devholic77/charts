
### redi 
* github repo : https://github.com/bitnami/charts/tree/master/bitnami/redis
* helm chart : https://charts.bitnami.com/bitnami
* values.yaml : https://github.com/bitnami/charts/blob/master/bitnami/redis/values.yaml

```sh
# repo 추가
> helm repo add bitnami https://charts.bitnami.com/bitnami

# 설치
> helm install redis bitnami/redis --values=./values.yaml

# 삭제
> helm delete mysql 
```
