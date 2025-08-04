# my-nginx-app
Sample Nginx App

## 部署步骤
### 部署应用
`helm install my-nginx-app ./my-nginx-app`
### 验证部署

``` yaml
# 查看部署状态
helm list

# 查看 Kubernetes 资源
kubectl get pods
kubectl get services

# 查看详细信息
helm status my-nginx-app
```

### 访问应用

`kubectl port-forward service/my-nginx-app 9000:80`

访问 `http://127.0.0.1:9000`

