# multi-service

## 安装
``` shell
helm install multiservice ./multi-service --set preInstallHook.enabled=false
```

## 查看 pod 启动顺序
``` shell
kubectl get pods -w
```