# GitLabCI Runner on Kubernetes 


## 自定义gitlab-runner  helm chart  
- chart version 0.15.0
- gitlab runner version 12.9.0

### 更新内容
- 添加构建缓存PVC
- 添加工作目录PVC
- 开启自定义构建目录


- buildcache-pvc.yml  构建缓存pvc配置
- buildsdir-pvc.yml   工作目录pvc配置
- gitlab-admin-user.yml gitlab&k8s集成用户（admin）


### 部署
```
helm install gitlab-runner04 ./gitlab-runner --namespace gitlab-runner
helm upgrade gitlab-runner04 ./gitlab-runner --namespace gitlab-runner

```

### 详细信息可以参考文档
