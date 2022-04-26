
### actions runner controller
github actions runner controller in k8s

* github repo : https://github.com/actions-runner-controller/actions-runner-controller
* helm chart : https://github.com/actions-runner-controller/actions-runner-controller/tree/master/charts/actions-runner-controller
* values.yaml : https://github.com/actions-runner-controller/actions-runner-controller/blob/master/charts/actions-runner-controller/values.yaml

---
* controller가 [cert-mananger](https://cert-manager.io/docs/installation/supported-releases/)를 사용하기 때문에 설치 필요


```sh
# cert-mananger 설치
> kubectl apply -f https://github.com/cert-manager/cert-manager/releases/download/v1.8.0/cert-manager.yaml

# repo 추가
> helm repo add actions-runner-controller https://actions-runner-controller.github.io/actions-runner-controller

# 설치
helm upgrade --install --namespace actions-runner-system --create-namespace actions-runner-controller actions-runner-controller/actions-runner-controller --values=./values.yaml

# 삭제
> helm delete actions-runner-controller --namespace actions-runner-system
```

### 