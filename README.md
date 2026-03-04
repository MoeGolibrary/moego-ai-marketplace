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
/plugin update moego
```
