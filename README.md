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
备用阿里镜像：registry.cn-hangzhou.aliyuncs.com/google_containers


##准备
- ansible>=2.4.0
- jinja2>=2.9.6
- netaddr
- pbr>=1.6
- ansible-modules-hashivault>=3.9.4
- hvac
- match
- register

```
#
# 安装pip
yum -y install epel-release
yum -y install python-pip  ansible
# 安装python-netaddr
pip install netaddr
pip install match
#Jinja 2.9 (or newer)
pip install --upgrade jinja2
systemctl stop firewalld
systemctl disable firewalld

#ssh-kengen
#ssh-copy-id   root@node1
