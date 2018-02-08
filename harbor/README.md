# 一、搭建一个Harbor私有镜像仓库:

[Harbor官网](https://vmware.github.io/harbor/cn/)，[Harbor下载页](https://github.com/vmware/harbor/releases)

## Master节点(10.100.1.31)搭建:

Master节点需要安装[docker](https://github.com/docker/docker-ce/releases)和[docker-compose](https://github.com/docker/compose/releases)

修改docker.service文件，添加以下内容：

```shell
--insecure-registry 10.100.1.31
```

# 二、Kubernetes集群需要用到的镜像：

## Pod镜像：

```shell
docker pull jaychiu/pod-infrastructure:rhel7
```

## Coredns镜像：

```shell
docker pull jaychiu/coredns:0.9.10
```

## Kube-router镜像：

```shell
docker pull jaychiu/kube-router:rhel7
```

## Dashboard镜像：

```shell
docker pull jaychiu/k8s-dashboard-amd64:head
```
# 三、Heapster插件需要用到的镜像：

## Heapster镜像：

```shell
docker pull jaychiu/heapster-amd64:v1.4.3
```

## Influxdb镜像：

```shell
docker pull jaychiu/heapster-influxdb-amd64:v1.1.1
```

## Grafana镜像：

```shell
docker pull jaychiu/heapster-grafana-amd64:v4.0.2
```

# 四、EFK插件需要用到的镜像：

## Elasticsearch镜像：

```shell
docker pull jaychiu/elasticsearch:v2.4.1-2
```

## Fluentd-elasticsearch镜像：

```shell
docker pull jaychiu/fluentd-elasticsearch:1.22
```

## Kibana镜像：

```shell
docker pull jaychiu/kibana:v4.6.1-1
```
# 五、MySQL需要用到的镜像：

## MySQL-master镜像：

```shell
docker pull jaychiu/mysql-master:5.7.21
```

## MySQL-slave镜像：

```shell
docker pull jaychiu/mysql-slave:5.7.21
```