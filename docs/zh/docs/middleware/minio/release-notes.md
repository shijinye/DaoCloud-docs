# MinIO 对象存储 Release Notes

本页列出 MinIO 对象存储的 Release Notes，便于您了解各版本的演进路径和特性变化。

## v0.1.4

发布日期：2022-11-28

- **改进** 更新获取前端的接口,增加 sc 列表是否可以扩容
- **改进** 密码校验调整为 MCamel 中等密码强度
- **新增** 创建 MinIO 集群时配置 Bucket
- **新增** 返回列表或者详情时的公共字段
- **新增** 返回告警列表
- **新增** 校验 Service 注释
- **修复** 创建 MinIO 时，密码校验从 between 调整为 length
- **改进** 完善优化复制功能
- **改进** 实例详情-访问设置，移除 集群 IPv4
- **改进** 中间件密码校验难度调整
- **新增** minio 支持创建的时候内置 BUCKET 创建
- **新增** 对接告警能力
- **新增** 新增判断 sc 是否支持扩容并提前提示功能
- **优化** 优化安装环境检测的提示逻辑&调整其样式
- **优化** 中间件样式走查优化

## v0.1.2

发布日期：2022-11-08

- **新增** 获取用户列表接口
- **新增** minio 实例创建
- **新增** minio 实例的修改
- **新增** minio 实例的删除
- **新增** minio 实例的配置修改
- **新增** minio 实例支持 nodeport 的 svc
- **新增** minio 实例的监控数据导出
- **新增** minio 实例的监控查看
- **新增** 多租户全局管理的对接
- **新增** mcamel-minio-ui 的创建/列表/修改/删除/查看
- **新增** APIServer/UI 支持 mtls
- **修复** 单例模式下，只有一个 pod，修复 grafana 无法获取数据问题
- **优化** 完善了计算器功能