---
weight: 41
bookCollapseSection: true
title: "4.1 容器运行时接口CRI"
---



容器运行时是现代容器化架构的基础组件，容器运行时接口 (CRI) 是一个插件接口，它允许 kubelet（Kubernetes 集群中每个节点上运行的代理）使用多种容器运行时。

CRI 最初是在 Kubernetes v1.5 中引入的；在引入 CRI 之前，kubernetes 直接将rkt 和 Docker 集成到 kubelet 的源代码中的，这使得用户将新的容器运行时与 Kubernetes 集成变得异常困难。 CRI就是在这种背景下诞生的，一方面kubernetes抽象出通用插件接口，专注于调度等功能，一方面，将适配工作下沉到了各个容器运行时开发人员。CRI 使 Kubernetes 用户能够轻松使用多个容器运行时，并使容器运行时的开发人员能够轻松地将它们与 Kubernetes 生态系统集成。





