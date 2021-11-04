# k8s
 
## 部署Node.js 应用
### Create pod
```
  kubectl run kubia --image=luksa/kubia --port=8080
```

### 暴露给外部
```
  kubectl expose pod kubia --type=NodePort --name=kubia-svc --port=80 --target-port=8080
  minikube service kubia-svc --url
  curl http://10.100.56.229:32569
```

  You've hit kubia.
 
 
