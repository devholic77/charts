### mysql
* github repo : https://github.com/bitnami/charts/tree/master/bitnami/mysql
* helm chart : https://bitnami.com/stack/mysql/helm
* values.yaml : https://github.com/bitnami/charts/blob/master/bitnami/mysql/values.yaml

```sh
# repo 추가
> helm repo add bitnami https://charts.bitnami.com/bitnami

# 설치
> helm install mysql bitnami/mysql --values=./values.yaml

# 셋팅된 password 확인
> ROOT_PASSWORD=$(kubectl get secret --namespace default mysql-devholic77 -o jsonpath="{.data.mysql-root-password}" | base64 --decode)

# 삭제
> helm delete mysql 
```
