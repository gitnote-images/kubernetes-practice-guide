# 目录

- [序言](README.md)

## 第一章: 排错指南

- [问题定位技巧](troubleshooting/debug-skill/README.md)
  - [分析 ExitCode 定位 Pod 异常退出原因](troubleshooting/debug-skill/analysis-exitcode.md)
  - [容器内抓包定位网络问题](troubleshooting/debug-skill/capture-packets-in-container.md)
  - [使用 systemtap 定位疑难杂症](troubleshooting/debug-skill/use-systemtap-to-locate-problems.md)
- [排错指引]()
  - [健康检查失败](troubleshooting/pod/healthcheck-failed.md)
  - [Pod 异常重启](troubleshooting/pod/pod-restart.md)
  - [Pod 一直 Pending](troubleshooting/pod/pod-pending-forever.md)
  - [Pod 一直 ContainerCreating](troubleshooting/pod/pod-containercreating-forever.md)
  - [Pod 一直 Terminating](troubleshooting/pod/pod-terminating-forever.md)
  - [无法登录容器](troubleshooting/pod/pod-cannot-exec-or-logs.md)
  - 无法查看容器日志
  - [TODO:Pod Terminating 慢](troubleshooting/pod/slow-pod-terminating.md)
  - [Job 无法被删除](troubleshooting/cannot-delete-job.md)
  - [no space left on device](troubleshooting/node/no-space-left-on-device.md)
  - [arp_cache: neighbor table overflow!](troubleshooting/node/arp_cache-neighbor-table-overflow.md)
  - [Cannot allocate memory](troubleshooting/node/cannot-allocate-memory.md)
  - [TODO:apiserver 响应慢]()
  - [TODO:ETCD频繁选主]()
  - [Service 访问不通](troubleshooting/network/service-unreachable.md)
  - [Service 无法解析](troubleshooting/network/service-cannot-resolve.md)
  - [LB 健康检查失败](troubleshooting/network/lb-healthcheck-failed.md)
  - [DNS 5秒延时](troubleshooting/network/dns-lookup-5s-delay.md)
  - [TODO:Pod 无法访问外网]()
  - [TODO:Pod 无法访问集群外的内网服务]()
  - [TODO:容器内无法 mount]()
- [处理实践]()
  - [节点 NotReady](troubleshooting/node/node-notready.md)
  - [Rancher 清除 Node 导致集群异常](troubleshooting/node/rancher-remove-node-cause-cluster-abnormal.md)
  - [内存碎片化](troubleshooting/node/memory-fragmentation.md)
  - [节点高负载](troubleshooting/node/high-load-on-node.md)
  - [驱逐导致服务中断](troubleshooting/node/eviction-leads-to-service-disruption.md)
  - [cgroup 泄露](troubleshooting/node/cgroup-leaking.md)
  - [inotify watch 耗尽](troubleshooting/node/runnig-out-of-inotify-watches.md)
  - [tcp_tw_recycle 导致在 NAT 环境会丢包](troubleshooting/node/lost-packets-in-nat-environment-once-enable-tcp_tw_recycle.md)

## 最佳实践

- [集群权限控制](best-practice/cluster-permission-control.md)
- [优雅热更新](best-practice/kubernetes-grace-update.md)
- [解决长连接服务扩容失效](best-practice/scale-keepalive-service.md)
- [使用 oom-guard 在用户态处理 cgroup OOM](best-practice/handle-cgroup-oom-with-oom-guard-in-userspace.md)
- [泛域名动态 Service 转发解决方案](best-practice/wildcard-domain-forward.md)
- [kubectl 高效技巧](best-practice/efficient-kubectl.md)
- [TODO:处理容器磁盘被写满](best-practice/handle-disk-full.md)
- [TODO:使用 MetalLB 创建负载均衡器]()
- [TODO:Pod 原地升级]()
- [TODO:Pod 固定 IP]()
- [TODO:使用 lxcfs 隔离 /proc]()
- [TODO:容器磁盘隔离]()

## K8S 配置管理

- [Helm]()
  - [安装 Helm](configuration-management/helm/install-helm.md)
  - [Helm V2 迁移到 V3](configuration-management/helm/upgrade-helm-v2-to-v3.md)
- [TODO:Kustomize]()

## 安全

- [cert-manager]()
  - [安装 cert-manager](security/cert-manager/install-cert-manger.md)
  - [使用 cert-manager 自动生成证书](security/cert-manager/autogenerate-certificate-with-cert-manager.md)

## Kubernetes 部署指南

- [TODO:二进制部署]()
- [TODO:使用 Kubeadm 部署]()
- [TODO:使用 Minikube 部署]()
- [TODO:使用 Bootkube 部署]()
- [TODO:使用 Ansible 部署]()

## K8S 管理工具

- [TODO:Rancher]()
- [TODO:Weave Scope]()
- [TODO:Kui]()
- [TODO:Kubernetes Dashboard]()
- [TODO:Kubetail]()
- [TODO:Kubebox]()

## 运行时

- [TODO:Docker]()
- [TODO:Containerd]()
- [TODO:CRI-O]()

## 服务发现

- [TODO:ETCD]()
- [TODO:Zookeeper]()
- [TODO:Consul]()

## 存储

- [ElasticSearch]()
  - [使用 elastic-oparator 部署 Elasticsearch 和 Kibana](storage/install-elasticsearch-and-kibana-with-elastic-oparator.md)
- [TODO:Rook]()
- [TODO:TiKV]()
- [TODO:ETCD]()
- [TODO:Zookeeper]()
- [TODO:Cassandra]()
- [TODO:MySQL]()
- [TODO:TiDB]()
- [TODO:PostgreSQL]()
- [TODO:MongoDB]()
- [TODO:InfluxDB]()
- [TODO:OpenTSDB]()

## 监控

- [TODO:Prometheus]()
- [TODO:Grafana]()
- [TODO:Jaeger]()

## Ingress

- [TODO:Nginx]()
- [TODO:Traefik]()
- [TODO:Envoy]()
- [TODO:Kong]()
- [TODO:Gloo]()
- [TODO:Contour]()
- [TODO:Ambassador]()
- [TODO:HAProxy]()
- [TODO:Skipper]()

## Service Mesh

- [TODO:Istio]()
- [TODO:Maesh]()
- [TODO:Kuma]()

## Serverless

- [TODO:Knative]()
- [TODO:Kubeless]()
- [TODO:Fission]()

## CI/CD

- [TODO:Jenkins X]()
- [TODO:Tekton]()
- [TODO:Argo]()
- [TODO:GoCD]()
- [TODO:GitLab CI]()

## 镜像相关

- [TODO:Harbor]()
- [TODO:Dragonfly]()
- [TODO:Kaniko]()
- [TODO:kpack]()

## 网络方案

- [TODO:Flannel]()
- [TODO:Macvlan]()
- [TODO:Calico]()
- [TODO:Cilium]()
- [TODO:Kube-router]()
- [TODO:Kube-OVN]()
- [TODO:OpenVSwitch]()