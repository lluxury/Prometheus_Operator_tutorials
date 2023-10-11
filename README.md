# Prometheus_tutorials
Prometheus_由少到多逐步实现

Prometheus 有本身和 Prometheus Operator 的区分，区别如下：

Prometheus Operator 
- k8s控制器，简化 Alertmanager、Grafana 的部署和管理
- 自动化
  - 自动创建和配置 Prometheus 实例
  - 自动处理 ServiceMonitors 和 PodMonitors
  - 提供 Prometheus 的升级和备份/还原功能
  - 自动创建 Alertmanager 和 Grafana 实例
- 复杂的 Kubernetes 集群

Prometheus
- 手动配置和管理 Prometheus 实例、Prometheus 配置文件、Alertmanager、Grafana
- 普通环境或定制化

遵循由简单到困难的方式，我们从Prometheus Operator开始实现。
麻烦牢记一个原则，对不熟悉的东西，不要从手动的方式开始接触，否则您很难看到全貌，相当长一段时间都是hello world 级别。

正确的做法是从正式的环境开始模仿，而不是简单的，这也是初学者和老手学习能力上的区别。
