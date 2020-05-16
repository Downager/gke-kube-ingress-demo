# gke-kube-ingress-demo

## 安裝 external 與 internal nginx ingress
```
helm upgrade --install ingress-nginx --namespace default ingress-nginx/
helm upgrade --install ingress-nginx-internal --namespace default ingress-nginx/ -f internal-values.yml
```
## 安裝 demo-app
```
helm upgrade --install demo-app --namespace default demo-app/
helm upgrade --install demo-app-internal --namespace default demo-app-internal/
```