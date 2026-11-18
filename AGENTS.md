# AGENTS.md · 项目规则

> 📌 **文档基线**：2026-11-18（commit `d2eca3c`）清理两条死链（obsidian-agent 已删除 / homekeeper → home-inventory）
> **更新索引后，请更新此行**（日期 + 新 commit hash），并在 CHANGELOG 追加。

## 本仓库定位（重要）
- `docker-tools` 是**索引仓库**：**只放文档，不放代码**。
- **自建服务 / Docker 应用**的**索引仓库（导航中心）**
- 各项目的源码 / 构建 / 发行都在**各自的独立仓库**里，本仓库只维护一张索引表。

## 约定
- 🔴 **不要**把任何项目源码、构建产物、发行包提交进本仓库
- 🔴 **不要**归档被索引的仓库 —— 归档后 **Releases 变只读，就发不了新版了**
- 🔒 私有仓库：在索引中**保留条目**便于本人一览，但**不给对外链接**（外部访问会 404）
- 新增条目：README 索引表按分类加一行 → CHANGELOG 加节
- 表格里的**最新版本 / 最近更新**取自各仓库的 Releases 与 push 时间，改版后记得同步
- 收录：可自托管的服务与应用（FastAPI / Django / Docker）


## 机器层（repo-kit · link-only）
- `tools/repo-kit/check_repo.py` 是**校验器**，不属于「工具源码」，与「本仓不放代码」不冲突
- 校验：`python tools/repo-kit/check_repo.py --root .`；锁哈希：`pwsh tools/update-repo-kit.ps1 -Check`
- 只查链接与锚点：四件套全部豁免 frontmatter，`include` 为空 = 扫全仓 `*.md`
- `schema/kit.lock.json` **不要手改**，升级只能跑 `tools/update-repo-kit.ps1`

## 相关
- 其它索引： [`pc-tools`](https://github.com/Simiely/pc-tools) · [`design-tools`](https://github.com/Simiely/design-tools) · [`mobile-apps`](https://github.com/Simiely/mobile-apps) · [`tech-guides`](https://github.com/Simiely/tech-guides) · [`docker-tools`](https://github.com/Simiely/docker-tools) · [`knowledge-hub`](https://github.com/Simiely/knowledge-hub)
- 领域总管仓库： [`ae-tools`](https://github.com/Simiely/ae-tools) · [`blender-addons`](https://github.com/Simiely/blender-addons) · [`c4d-tools`](https://github.com/Simiely/c4d-tools)
