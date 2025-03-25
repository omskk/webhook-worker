# Cloudflare Worker Scheduled Task

## 📌 项目简介

本项目使用 Cloudflare Workers 运行定时任务（Scheduled Event），定期调用指定 API（`SENDURL`）并打印返回结果。

---

## 🚀 部署步骤

### 1️⃣ Fork GitHub 仓库

1. 在 GitHub 上 fork 本项目的代码。
2. 进入 Cloudflare Workers 控制台。

### 2️⃣ 直接部署到 Cloudflare Workers

1. 选择 `Create a Worker`。
2. 选择 `Deploy from GitHub`，连接你的 fork 仓库。
3. 部署 Worker，无需修改代码。

### 3️⃣ 配置环境变量

1. 进入 Cloudflare Workers 的 `Settings` → `Variables`。
2. 添加变量：
   - **`SENDURL`** = 你的目标 API 地址。

### 4️⃣ 配置定时任务（Scheduled Events）

1. 进入 `Triggers` 选项卡。
2. 添加 Cron 触发器，例如 `*/5 * * * *`（每 5 分钟执行一次）。

---

## 📝 其他信息

- Cloudflare Workers 文档：[官方文档](https://developers.cloudflare.com/workers/)
- Cloudflare Dashboard：[管理页面](https://dash.cloudflare.com/)

💡 **如果遇到问题，可以在 Issue 区提问，或参考 Cloudflare 官方文档！** 🚀

