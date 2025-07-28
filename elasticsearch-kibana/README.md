# elasticsearch + kibana
Sample Elasticsearch and Kibana

## 部署步骤
### 部署应用
`helm install my-elastic ./elasticsearch-kibana`
### 验证部署

``` yaml
# 查看部署状态
helm list

# 查看 Kubernetes 资源
kubectl get pods
kubectl get svc

# 查看详细信息
helm status my-elastic
```

### 访问应用

`kubectl port-forward svc/my-elastic-elasticsearch-kibana-elasticsearch 9200:9200`

访问 `http://127.0.0.1:9000`

