# k8s-install

来自项目 https://github.com/kubesphere/kubesphere

> sshpass 不持密码



## 有修改
* /k8s/inventory/sample/group_vars/k8s-cluster/k8s-cluster.yml
调整为国内镜像
```
# kubernetes image repo define
kube_image_repo: "gcr.azk8s.cn/google-containers"
```
