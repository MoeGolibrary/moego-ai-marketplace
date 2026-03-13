# MoeGo AI Marketplace

MoeGo 研发团队 Claude Code Plugin Marketplace。

本仓库仅存放 marketplace 配置（插件目录），不含 plugin 代码。Plugin 代码在 [moego-ai-plugin](https://github.com/MoeGolibrary/moego-ai-plugin)。

> 想添加新 Skill？请到 [moego-ai-plugin](https://github.com/MoeGolibrary/moego-ai-plugin) 仓库提交 PR。本仓库只在 plugin 发版时更新 version 和 ref。

## 安装

```bash
# 1. 添加 Marketplace（一次性）
/plugin marketplace add MoeGolibrary/moego-ai-marketplace

# 2. 安装 Plugin
/plugin install moego@moego-ai-marketplace
```

安装后可用的 Skill 列表见 [moego-ai-plugin README](https://github.com/MoeGolibrary/moego-ai-plugin#readme)。

## 更新

```bash
# 更新 Marketplace 目录（获取最新插件列表）
/plugin marketplace update

# 更新 Plugin（拉取插件最新版本）
/plugin update moego
```

## 发版流程

当 plugin 仓库发布新版本时，需同步更新本仓库：

1. 修改 `marketplace.json` 中的 `version` 和 `source.ref` 为新版本号
2. 提交 PR 合入 `production` 分支

## 注意事项

- 本 Marketplace 的 GitHub 默认分支为 `production`，`/plugin marketplace add` 会拉取该分支
- Plugin 版本锁定在 git tag，更新版本时需同步修改 marketplace.json 中的 `version` 和 `ref`
