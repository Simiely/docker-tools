# docker-tools · 自建服务 / Docker 索引

> 🔖 **本仓库是索引仓库（导航中心），不放任何代码。**
> 每个服务都在它**自己的独立仓库**里（多数可 Docker 一键部署）—— 点下表链接直达。

## 服务一览

| 服务 | 说明 | 技术栈 | 最近更新 |
|---|---|---|---|
| **[`homekeeper`](https://github.com/Simiely/homekeeper)** | 家居物品管理：记录物品**位置 / 保质期 / 状态**，Docker 一键部署、浏览器访问 | FastAPI + SQLite + 原生 JS | 2026-08-08 |
| **[`obsidian-agent`](https://github.com/Simiely/obsidian-agent)** | Docker 化的 Obsidian 知识库 AI 助手：指定 vault 路径即可浏览、编辑、全文检索全部 Markdown | Python · Docker | 2026-08-14 |
| **[`learning-platform`](https://github.com/Simiely/learning-platform)** 🔗[页面](https://simiely.github.io/learning-platform/) | Lets Learn：幼儿识字 / 认知闪卡平台，支持浏览、卡片、练习三种模式，为触屏优化 | Django + Alpine.js | 2026-08-03 |

## 说明

- **一个服务一个仓库**：源码、Issue、部署说明都在各自仓库；本仓库只负责**索引与导航**；
- **为什么不归档**：这些服务仍在独立迭代，归档后 Releases 亦变只读，因此统一为「各仓库独立 + 本仓做索引」；
- 文档规范参照 [`knowledge-base`](https://github.com/Simiely/knowledge-base) 单项目规范（该仓独立维护）。

## 相关仓库

- 平台层：[`tools-center`](https://github.com/Simiely/tools-center)（轻量工具统一宿主，跑在 NAS 上）
- 其它索引：[`pc-tools`](https://github.com/Simiely/pc-tools)（PC 端）· [`design-tools`](https://github.com/Simiely/design-tools)（设计 / 3D）· [`mobile-apps`](https://github.com/Simiely/mobile-apps)（移动端）· [`tech-guides`](https://github.com/Simiely/tech-guides)（技术文档）· [`knowledge-hub`](https://github.com/Simiely/knowledge-hub)（知识库）
