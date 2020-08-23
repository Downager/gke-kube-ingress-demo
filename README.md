# gke-kube-ingress-demo

## 說明
請參考 [blog 文章](https://blog.downager.com/2020/05/17/Kubernetes-%E5%9C%A8-GKE-%E4%B8%8A%E5%90%8C%E6%99%82%E5%95%9F%E7%94%A8-internal-%E8%88%87-external-%E5%85%A9%E7%A8%AE-nginx-ingress-controller/)

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
