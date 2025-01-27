# 插件中心介绍

插件中心是针对云原生网关和云原生微服务的统一插件管理门户，其中涉及多种流控，权限及自定义插件，
一次配置后即可在云原生网关和云原生微服务中进行使用，避免了相同业务逻辑需求下的插件重复开发，为开发和运维人员带来了更多便利。

微服务引擎支持接入 Auth、JWT、全局限流、Wasm 插件。
**只有先在插件中心接入插件，然后才能在云原生微服务或云原生网关中使用这些插件** 。

- JWT（JSON Web Token）是一种用于身份验证和授权的开放标准。它由三部分组成：
头部、载荷和签名。JWT 可以在客户端和服务器之间传递信息，并使用签名进行验证。
在云计算和云原生行业中，JWT 通常用于在微服务架构中进行身份验证和授权。

- Auth（Authorization）是一种用于验证用户身份和授权访问的插件。
它可以与 JWT 一起使用，对请求进行身份验证，并根据用户的权限决定是否允许访问特定资源。
Auth 插件可以确保只有经过身份验证的用户才能访问特定的 API 或服务。

- Rate Limit（全局限流）是一种用于限制请求速率的插件。在云计算和云原生环境中，
由于大量的请求可能会对系统造成负载压力，Rate Limit 插件可以帮助限制每个用户或 IP 地址的请求速率，以确保系统的稳定性和安全性。

- Wasm（WebAssembly）是一种低级别的字节码格式，可以在浏览器中运行高性能的编译代码。
在云计算和云原生行业中，Wasm 可以用作插件的运行环境，使开发人员能够使用更多的编程语言和工具来扩展和定制云服务。
通过使用 Wasm 插件，可以实现更高效、可扩展和灵活的云原生应用程序。

![plugin list](https://docs.daocloud.io/daocloud-docs-images/docs/zh/docs/skoala/images/plugin01.png)
