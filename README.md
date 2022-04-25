# argocd-helm-app-of-apps
App of APPS 패턴의 child 폴더(app-of-apps)를 helm template 으로 개발했습니다.

#### create apps
```bash
kubectl apply -f apps.yaml
```

#### delete apps
```bash
kubectl delete -f apps.yaml
```