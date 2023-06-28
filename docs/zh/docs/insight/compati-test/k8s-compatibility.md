# Kubernetes 集群兼容性测试

✅：测试通过；  ❌：测试未通过。

!!! note

    表格中的测试功能非全量。

|   case           |        |  测试方式       | K8s 1.26 |k8s 1.23.0 ~ 1.23.13 | k8s 1.24.0 ~ 1.24.7  | k8s 1.25.0 ~ 1.25.3  | k8s 1.22 | k8s 1.21| k8s 1.20| k8s 1.19|k8s 1.18 |备注  |
| ------------ | ------------------------ | ---------------- | --------- | --------- | --------- | --------- | --------- | --------- |--------- |--------- |--------- |--------- |
| 采集并查询 web 应用的指标 |            |   E2E          | ✅ | ✅      | ✅      | ✅     | ✅ | ✅| ✅| ✅| |     | 
| 添加自定义指标采集  |     |  E2E           | ✅ | ✅      | ✅      | ✅      | ✅ | ✅| ✅| ✅| |       | 
| 查询实时指标  |     |    E2E           | ✅ | ✅      | ✅      | ✅      | ✅ | ✅| ✅| ✅| |       | 
| 瞬时指标查询   |     |    E2E          | ✅ | ✅      | ✅      | ✅      | ✅ | ✅| ✅| ✅| |      |
| 瞬时指标api字段功能验证   |     |    E2E          | ✅ | ✅      | ✅      | ✅      | ✅ | ✅| ✅| ✅| |      |
| 查询一段时间内指标   |     |    E2E          | ✅ | ✅      | ✅      | ✅      | ✅ | ✅| ✅| ✅| |      |
| 查询一段时间内指标 api 字段功能验证   |     |    E2E           | ✅ | ✅      | ✅      | ✅      | ✅ | ✅| ✅| ✅| |      |
| 批量查询集群CPU、内存使用率、集群 CPU 总量、集群内存使用量，集群节点总数   |     |    E2E           | ✅ | ✅      | ✅      | ✅      | ✅ | ✅| ✅| ✅| |      |
| 批量查询节点CPU、内存使用率、节点 CPU 总量、节点内存使用量   |     |    E2E           | ✅ | ✅      | ✅      | ✅      | ✅ | ✅| ✅| ✅| |      |
| 批量查询一段时间内的集群CPU、内存使用率、集群 CPU 总量、集群内存使用量，集群节点总数  |     |    E2E    | ✅ | ✅      | ✅      | ✅     | ✅ | ✅| ✅| ✅|  |      |
| 批量查询查询一段时间内指标 api 字段功能验证  |     |    E2E           | ✅ | ✅      | ✅      | ✅    | ✅ | ✅| ✅| ✅ |      |
| 查询 Pod 日志   |     |    E2E           | ✅ | ✅      | ✅      | ✅      | ✅ | ✅| ✅| ✅| |       |
| 查询 SVC 日志  |     |    E2E           | ✅ | ✅      | ✅      | ✅     | ✅ | ✅| ✅| ✅|  |       |
| 查询 statefulset 日志  |     |    E2E  | ✅ | ✅      | ✅      | ✅     | ✅ | ✅| ✅| ✅|  |       |
| 查询 Deployment 日志  |     |    E2E | ✅ | ✅      | ✅      | ✅     | ✅ | ✅| ✅| ✅|  |       | 
| 查询 NPD 日志     |     |    E2E     | ✅ | ✅      | ✅      | ✅     | ✅ | ✅| ✅| ✅|  |       |
| 日志筛选  |     |    E2E          | ✅ | ✅      | ✅      | ✅     | ✅ | ✅| ✅| ✅|  |       |
| 日志模糊查询-workloadSearch   |     |    E2E          | ✅ | ✅      | ✅      | ✅      | ✅ | ✅| ✅| ✅| |      |
| 日志模糊查询-podSearch   |     |    E2E          | ✅ | ✅      | ✅      | ✅      | ✅ | ✅| ✅| ✅| |      |
| 日志模糊查询-containerSearch   |     |    E2E          | ✅ | ✅      | ✅      | ✅     | ✅ | ✅| ✅| ✅|  |      |
| 日志精确查询-cluster   |     |    E2E          | ✅ | ✅      | ✅      | ✅    | ✅ | ✅| ✅| ✅|   |      |
| 日志精确查询-namespace  |     |    E2E          | ✅ | ✅      | ✅      | ✅     | ✅ | ✅| ✅| ✅|  |      |
| 日志查询 api 字段功能验证   |     |    E2E          | ✅ | ✅      | ✅      | ✅    | ✅ | ✅| ✅| ✅|   |      |