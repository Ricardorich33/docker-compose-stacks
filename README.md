# docker-compose-stacks

常用服务的 Docker Compose 部署模板，适合测试环境和中小规模部署。

## 目录

- `monitoring/`：Prometheus + Node Exporter + Alertmanager + Grafana。
- `web-app/`：Nginx 反向代理 + 应用 + Redis + MySQL 的示例编排。

## 使用

```bash
cd monitoring
docker compose up -d
```

## 注意事项

- 生产使用请替换默认密码、挂载持久化目录，并配置资源限制。
- 模板里的版本号、路径和端口按实际环境调整。
