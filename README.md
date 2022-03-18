# argocd-helm-app-of-apps

#### kubectl 명령어 사용
```bash
kubectl apply -f main.yaml
```

#### OR
#### argocd cli 사용 (BEST!)
```bash
argocd app create aaa-main --repo https://github.com/jenana-devops/argocd-helm-app-of-apps.git \
--path child --revision HEAD \
--dest-namespace default --dest-server https://kubernetes.default.svc
```

#### OR
#### helm 사용
```bash
helm install aaa main -n <ns>
```

#### delete app
```bash
argocd app delete aaa-main
```