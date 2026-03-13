# MoeGo AI Marketplace

MoeGo 研发团队 Claude Code Plugin Marketplace。

## 安装

```bash
# 1. 添加 Marketplace（一次性）
/plugin marketplace add MoeGolibrary/moego-ai-marketplace

# 2. 安装 Plugin
/plugin install moego@moego-ai-marketplace
```

## 可用 Plugin

| Command | 说明 |
|---------|------|
| `/moego:superflow` | AI Native 开发工作流（功能开发 → PR 交付） |
| `/moego:e2e` | E2E 测试规划与 Playwright 代码生成 |
| `/moego:datadog` | Datadog 日志/Trace/服务依赖查询 |
| `/moego:writing-prompts` | 编写 LLM 一次性 Prompt |
| `/moego:writing-system-documents` | 编写 Agent 常驻系统文档 |

## 更新

```bash
# 更新 Marketplace 目录（获取最新插件列表）
/plugin marketplace update

# 更新 Plugin（拉取插件最新版本）
/plugin update moego
```

## 注意事项

- 本 Marketplace 的 GitHub 默认分支为 `production`，`/plugin marketplace add` 会拉取该分支
- Plugin 版本锁定在 `v2.0.0` tag，更新版本时需同步修改 marketplace.json 中的 `version` 和 `ref`
