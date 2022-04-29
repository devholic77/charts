### jenkins 
* github repo : https://github.com/jenkinsci/helm-charts/tree/main/charts/jenkins
* values.yaml : https://github.com/argoproj/argo-helm/blob/master/charts/argo-cd/values.yaml

```sh
# repo 추가
> helm repo add jenkins https://charts.jenkins.io
> helm repo update

# 설치
> helm install jenkins jenkins/jenkins --values=./values.yaml

# 삭제
> helm delete jenkins 
```
