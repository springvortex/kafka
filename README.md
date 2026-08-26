# Kafka 零基础实战指南

这是部署在 `uhaiin.com/kafka/` 的 Kafka 阅读站。内容从 KRaft 集群和第一条消息开始，覆盖生产者消费者、分区与副本、事务语义、KRaft 元数据、性能调优、安全运维、Connect 与 Streams 生态和事件驱动架构。

## 站点信息

| 项 | 值 |
|---|---|
| 线上地址 | `https://uhaiin.com/kafka/` |
| `baseurl` | `/kafka` |
| 文章数 | 29 篇 |
| 发布日期 | 2026-01-01 至 2026-01-29 |
| License | Apache-2.0 |

## 内容路径

- `_posts/`：28 章正文和 1 篇速查手册，每章一篇博客。
- `_config.yml`：站点标题、路径、导航、访问计数和推荐阅读配置。
- `static/`：站点样式、脚本、图片和生成的静态资源。
- `.github/workflows/`：GitHub Pages 的 Jekyll 构建、热门文章生成、压缩和检查流程。

内容覆盖主题分区管理、序列化与 Schema Registry、Spring Boot 集成、日志分段索引、ISR 与高可用、Controller、Purgatory、幂等事务与 Exactly Once、Rebalance、KRaft、容量规划、可靠性清单、监控告警、故障排查、认证加密授权、扩容迁移升级和日志平台实战。

## 本地预览

```bash
bundle install
npm ci
./blog.sh run
```

默认访问 `http://localhost:8080/kafka/`。`blog.sh` 是 Bash 脚本，Windows 下建议在 Git Bash 或 WSL 中执行。

## 维护约定

- 新增或修订章节时只改 `_posts/`，保持文件名日期和章节顺序一致。
- 不要改 `_config.yml` 中的 `baseurl: '/kafka'`；RSS、canonical、sitemap 和静态资源地址都依赖它。
- 推送 `main` 后，GitHub Actions 会自动构建并发布站点。
