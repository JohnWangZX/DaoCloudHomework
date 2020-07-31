开发一个 Spring Boot 应用



## 功能要求：(15)

1.1 实现一个 REST 接口（简单接口即可，比如 json 串 {"msg":"hello"}）(2)☑️

1.2 接口提供限流功能，当请求达到每秒 100 次的时候，返回 429（Too many requests）(8)☑️

1.3 加分项：当后端服务有多个实例的时候（一个 Service 包含若干个 Pod），如何实现统一限流(bonus 5)



## DevOps 要求：(25)

2.1 为该项目准备 Dockerfile，用于构建镜像(2)

2.2 为该项目准备 K8s 编排文件，用于在 K8s 创建服务（service）(3)

2.3 准备 Jenkins 持续集成流水线，实现代码构建/单元测试/镜像构建功能(10)

2.4 准备 Jenkins 持续部署流水线，实现部署到 K8s 集群的功能，该流水线的触发条件为持续集成流水线执行成功(5)

2.5 准备 Jenkins 持续测试流水线，基于 RTF 实现自动接口测试，该流水线的触发条件为持续部署流水线执行成功(5)



## 扩容场景：(20)

3.1 为该项目提供 Prometheus metrics 接口，可以供 Prometheus 采集监控指标(5)

3.2 在 Grafana 中的定制应用的监控大屏(5)

3.3 使用压测工具（例如 Jmeter）对接口进压测，观察 Grafana 监控数据(5)

3.4 通过 Kubernetes 命令进行手工扩容，并再次观察 Grafana 监控数据(5)

3.5 加分项：使用 K8s HPA 模块根据 CPU 负载做服务的 Auto Scale(5)