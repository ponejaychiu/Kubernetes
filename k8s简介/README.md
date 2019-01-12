# Kubernetes
此目录是用来学习k8s技术的，包含相关技术操作文档。

# 中文学习文档
https://www.kubernetes.org.cn/docs

https://jimmysong.io/kubernetes-handbook

# Kubernetes主要由以下几个核心组件组成：

 **etcd** 保存了整个集群的状态；

 **apiserver** 提供了资源操作的唯一入口，并提供认证、授权、访问控制、API注册和发现等机制；

 **controller manager** 负责维护集群的状态，比如故障检测、自动扩展、滚动更新等；

 **scheduler** 负责资源的调度，按照预定的调度策略将Pod调度到相应的机器上；

 **kubelet** 负责维护容器的生命周期，同时也负责Volume（CVI）和网络（CNI）的管理；

 **Container runtime** 负责镜像管理以及Pod和容器的真正运行（CRI）；

 **kube-proxy** 负责为Service提供cluster内部的服务发现和负载均衡；> 这里输入引用文本

# 除了核心组件，还有一些推荐的Add-ons：

 **kube-dns** 负责为整个集群提供DNS服务；

 **Ingress Controller** 为服务提供外网入口；

 **Heapster** 提供资源监控；

 **Dashboard** 提供GUI；

 **Federation** 提供跨可用区的集群；

 **Fluentd-elasticsearch** 提供集群日志采集、存储与查询
