# Kafka：从 0 基础到大师

这是以 `demo/` 为只读模板生成的独立 Jekyll 阅读站。原书目录是 `../kafka-0基础到大师/`，本仓库负责把书稿按章节发布成博客站点。

## 生成结果

| 项 | 值 |
|---|---|
| 站点标题 | Kafka：从 0 基础到大师 |
| 站点路径 | `https://uhaiin.com/kafka/` |
| `baseurl` | `/kafka` |
| 访问计数命名空间 | `uhaiin.com/kafka` |
| 博客文章数 | 29 |
| 内容来源 | `../kafka-0基础到大师/` |

章节文件来自书稿中的 `01-*.md` 到最后章节以及 `appendix-速查手册.md`，每章一篇博客。文章按发布日期顺序生成，标题保留章号和章节名。

## 本地预览

```bash
bundle install
npm ci
./blog.sh run
```

默认访问 `http://localhost:8080/kafka/`。`blog.sh` 是 Bash 脚本，Windows 下建议在 Git Bash 或 WSL 中执行。

## 路径配置

本站运行在 `https://uhaiin.com/kafka/`。模板中 `domainUrl` 与 `baseurl` 会拼接生成 canonical、RSS、sitemap 和静态资源地址，因此采用标准 Jekyll 项目路径配置：

```yaml
url: 'https://uhaiin.com/kafka'
domainUrl: 'https://uhaiin.com'
baseurl: '/kafka'
```

其中 `url` 保存书籍站点的完整地址；模板实际输出 canonical、RSS 和 sitemap 时，使用 `domainUrl + baseurl`，因此 `domainUrl` 保留域名根地址，避免 `/kafka/kafka/` 这种重复路径。

访问计数与 CI 生成热门文章时使用 `uhaiin.com/kafka` 命名空间，避免和其他书站的数据混在一起。

## 部署

仓库保留了 GitHub Pages Actions 流程。推送 `main` 分支后，Actions 会执行 Jekyll 构建、评论索引生成、热门文章生成、压缩和站点检查。

GitHub Pages 的 `Source` 需要选择 `GitHub Actions`。如果使用项目仓库路径或反向代理子路径部署，必须保持 `baseurl: '/kafka'`。