# 搭建一个harbor镜像仓库:

## Master节点(10.100.1.31)搭建:

Master节点需要安装docker和docker-compose

修改docker.service文件，添加以下内容：

`--insecure-registry 10.100.1.31`

## Pod镜像：

`docker pull registry.access.redhat.com/rhel7/pod-infrastructure:latest`

## coredns镜像：

`docker pull registry.docker-cn.com/coredns/coredns:0.9.10`

## kube-router镜像：

`docker pull cloudnativelabs/kube-router:latest`

## dashboard镜像：

`docker pull registry.docker-cn.com/kubernetesdashboarddev/kubernetes-dashboard-amd64:head`