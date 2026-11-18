# CHANGELOG.md · 仓库级变更

## 仓库 · 2026-11-18 · 接入 repo-kit 机器层（link-only）

### 新增

- `schema/taxonomy.json` + `schema/kit.lock.json`（kit `2.8.1` / 规范 `2.1.4` / `link-only`）
- `tools/repo-kit/check_repo.py`、`tools/update-repo-kit.ps1`
- `.github/workflows/repo-check.yml`：push 到 main 与 PR 时跑链接/锚点检查 + 锁哈希校验

### 说明

- 只查「链接是否可达、锚点是否存在」，不要求 frontmatter（四件套全部豁免）。
  本仓是索引仓，真正的风险是仓库链接 404——上午那次死链是**手工**发现的，现在有门禁。
- `tools/repo-kit/` 是校验器，不算「工具源码」，与「本仓不放代码」不冲突。

## 仓库 · 2026-11-18 · 清理两条死链

### 修复

- **撤掉 `obsidian-agent` 条目**：仓库已于 2026-11-18 删除（本人确认不再维护），索引里的链接变成 404
- **`homekeeper` 改为 `home-inventory`**：homekeeper 已于 2026-10-27 删除、功能由 home-inventory 取代（见 knowledge-base 用户库/仓库盘点表「已删除」区），本索引一直没跟上；home-inventory 有 `Dockerfile` + `docker-compose.yml`，仍属本仓收录范围
- 两条都是「链到不存在的仓库」的硬 404，不是内容过期；顺手核对 README 里其余 8 条仓库链接，均有效

## 仓库 · 2026-10-09 · 建库

### 建库

- 建立索引仓库（纯文档、零代码），收录下列项目：
- 收录：可自托管的服务与应用（FastAPI / Django / Docker）

