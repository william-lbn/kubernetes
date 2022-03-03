---
weight: 41
bookCollapseSection: true
title: "4.1 容器运行时接口CRI"
---



容器运行时接口 (CRI) 是一个插件接口，它允许 kubelet（在 Kubernetes 集群中的每个节点上运行的代理）使用多种容器运行时。容器运行时是现代容器化架构的基础组件。

CRI 最初是在 Kubernetes v1.5 中引入的。在引入 CRI 之前，rkt 和 Docker 是直接集成到 kubelet 的源代码中的。这使得将新的容器运行时与 Kubernetes 集成变得困难。 CRI 使 Kubernetes 用户能够轻松使用多个容器运行时，并使容器运行时的开发人员能够轻松地将它们与 Kubernetes 生态系统集成。





