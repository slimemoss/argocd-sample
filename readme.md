# argocdのインストール
```
kubectl create namespace argocd-sample
https://raw.githubusercontent.com/argoproj/argo-cd/stable/manifests/install.yaml | sed "s@quay.io/argoproj/argocd@alinbalutoiu/argocd@g" | kubectl apply -n argocd-sample -f 
```

# 管理するリポジトリの登録
```
```

# argocdのアンインストール
```
https://raw.githubusercontent.com/argoproj/argo-cd/stable/manifests/install.yaml | sed "s@quay.io/argoproj/argocd@alinbalutoiu/argocd@g" | kubectl delete -n argocd-sample -f 
kubectl delete namespace argocd-sample
```
