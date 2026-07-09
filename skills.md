# Skills 索引

常用 Agent Skills 功能简介与来源。本地路径以 `~` 表示用户主目录。

> **安装说明**
> - Cursor Skills：`~/.cursor/skills/`（用户级）或 `.cursor/skills/`（项目级）
> - Cursor 内置 Skills：`~/.cursor/skills-cursor/`（随 Cursor 更新）
> - Agents Skills：`~/.agents/skills/`
> - Codex Skills：`~/.codex/skills/`

---

## 开发流程

| Skill | 功能简介 | 仓库 / 来源 | 本地路径 |
|-------|----------|-------------|----------|
| `superpowers-workflow` | 编排完整软件开发流程：头脑风暴 → 设计审批 → 详细计划 → TDD 执行 → 代码审查 | [obra/superpowers](https://github.com/obra/superpowers) | `~/.cursor/skills/superpowers-workflow/` |
| `superpowers-brainstorming` | 编码前设计头脑风暴，经用户审批后再进入实现 | [obra/superpowers/skills/brainstorming](https://github.com/obra/superpowers/tree/main/skills/brainstorming) | `~/.cursor/skills/superpowers-brainstorming/` |
| `superpowers-writing-plans` | 编写含文件路径、代码片段与验证命令的详细实现计划 | [obra/superpowers/skills/writing-plans](https://github.com/obra/superpowers/tree/main/skills/writing-plans) | `~/.cursor/skills/superpowers-writing-plans/` |
| `superpowers-executing-plans` | 在当前会话中执行已写好的计划，用 TodoWrite 跟踪进度 | [obra/superpowers/skills/executing-plans](https://github.com/obra/superpowers/tree/main/skills/executing-plans) | `~/.cursor/skills/superpowers-executing-plans/` |
| `create-plan` | 快速生成只读执行计划（适合单次回复的 checklist） | [openai/skills](https://github.com/openai/skills/tree/main/skills/.experimental/create-plan) | `~/.cursor/skills/create-plan/` |
| `dev-log-archive` | 开发过程中实时追加 `dev_log` 日归档，记录背景、需求、过程与结果 | 项目自定义 | `~/.cursor/skills/dev-log-archive/` |

---

## 代码理解（Understand Anything）

上游项目：[Lum1104/Understand-Anything](https://github.com/Lum1104/Understand-Anything)（MIT）

| Skill | 功能简介 | 本地路径 |
|-------|----------|----------|
| `understand-anything` | 路由入口：多 Agent 代码分析、知识图谱、diff 影响、领域流、wiki 图谱 | `~/.cursor/skills/understand-anything/` |
| `understand` | 分析代码库，生成交互式架构知识图谱 | `~/.cursor/skills/understand/` |
| `understand-chat` | 基于知识图谱对代码库提问与对话 | `~/.cursor/skills/understand-chat/` |
| `understand-dashboard` | 启动 Web 仪表盘可视化知识图谱 | `~/.cursor/skills/understand-dashboard/` |
| `understand-diff` | 分析 git diff / PR 变更、影响组件与风险 | `~/.cursor/skills/understand-diff/` |
| `understand-domain` | 提取业务领域知识，生成交互式领域流程图 | `~/.cursor/skills/understand-domain/` |
| `understand-explain` | 对指定文件、函数或模块做深度解读 | `~/.cursor/skills/understand-explain/` |
| `understand-knowledge` | 分析 Karpathy 模式 LLM wiki，生成知识图谱 | `~/.cursor/skills/understand-knowledge/` |
| `understand-onboard` | 为新成员生成项目 onboarding 指南 | `~/.cursor/skills/understand-onboard/` |

**安装：** `bash ~/.cursor/skills/understand-anything/scripts/install-cursor.sh`，或在 Cursor Settings → Plugins 添加 `https://github.com/Lum1104/Understand-Anything`。

---

## Cursor 内置 Skills

来源：Cursor 官方内置（`~/.cursor/skills-cursor/`），随 IDE 更新。

| Skill | 功能简介 | 文档 |
|-------|----------|------|
| `automate` | 创建 Cursor Automations（定时/触发式 Agent 任务） | [Cursor Automations](https://cursor.com/docs/agent/automations) |
| `babysit` | 看护 PR：处理评论、解决冲突、修复 CI 直至可合并 | — |
| `canvas` | 生成交互式 Canvas（React 应用），用于数据分析、审计、图表等 | — |
| `create-hook` | 创建 Cursor Hooks（`hooks.json` 与钩子脚本） | [Cursor Hooks](https://cursor.com/docs/agent/hooks) |
| `create-rule` | 创建 Cursor Rules（`.cursor/rules/*.mdc`） | [Cursor Rules](https://cursor.com/docs/context/rules) |
| `create-skill` | 编写 Agent Skill（`SKILL.md` 结构与最佳实践） | [Cursor Skills](https://cursor.com/docs/context/skills) |
| `create-subagent` | 创建自定义 Subagent（专用审查、调试等） | — |
| `loop` | 按间隔循环执行 prompt 或 skill（如 `/loop 5m /foo`） | — |
| `migrate-to-skills` | 将 `.mdc` Rules 和 slash commands 迁移为 Skills 格式 | — |
| `review` | 选择 Bugbot 或 Security Review 子代理审查代码 | — |
| `review-bugbot` | 用 Bugbot 子代理审查代码变更 | — |
| `review-security` | 用 Security Review 子代理做安全审查 | — |
| `sdk` | 基于 Cursor SDK（`@cursor/sdk` / `cursor-sdk`）构建自动化集成 | [SDK TypeScript](https://cursor.com/docs/sdk/typescript) · [SDK Python](https://cursor.com/docs/sdk/python) |
| `shell` | 终端命令执行规范与最佳实践 | — |
| `split-to-prs` | 将当前工作拆分为多个可审查的小 PR | — |
| `statusline` | 配置 CLI 自定义状态行 | — |
| `update-cli-config` | 修改 Cursor CLI 配置 | — |
| `update-cursor-settings` | 修改 Cursor / VSCode `settings.json` | — |

---

## 产品 / 商业分析

来源：`~/.agents/skills/`（部分改编自 [deanpeters/product-manager-prompts](https://github.com/deanpeters/product-manager-prompts)）

| Skill | 功能简介 | 本地路径 |
|-------|----------|----------|
| `company-research` | 生成公司调研简报：高管观点、产品战略、组织背景 | `~/.agents/skills/company-research/` |
| `competitive-analysis` | 系统性竞品分析：产品、定价、定位、市场策略 | `~/.agents/skills/competitive-analysis/` |
| `competitive-intel` | 竞品情报跟踪，输出销售 battlecard 与定位建议 | `~/.agents/skills/competitive-intel/` |
| `feature-prioritization-assistant` | 用 RICE 模型做功能优先级排序 | `~/.agents/skills/feature-prioritization-assistant/` |
| `market-research` | 市场调研、竞品对比、行业情报（附来源引用） | `~/.agents/skills/market-research/` |
| `prd-development` | 结构化 PRD 撰写：问题、用户、方案、成功指标 | `~/.agents/skills/prd-development/` |
| `prd-writer` | 生成完整产品需求文档 | `~/.agents/skills/prd-writer/` |
| `product-strategy-session` | 端到端产品战略研讨：定位、发现、路线图 | `~/.agents/skills/product-strategy-session/` |
| `roadmap-planning` | 战略路线图规划：优先级、Epic、排期 | `~/.agents/skills/roadmap-planning/` |
| `saas-metrics-coach` | SaaS 财务健康顾问（ARR、MRR、Churn、LTV、CAC 等） | `~/.agents/skills/saas-metrics-coach/` |

---

## 知识管理（Basic Memory）

上游项目：[basicmachines-co/basic-memory](https://github.com/basicmachines-co/basic-memory)

| Skill | 功能简介 | 本地路径 |
|-------|----------|----------|
| `memory-notes` | 编写结构化 Basic Memory 笔记（frontmatter、observations、relations） | `~/.agents/skills/memory-notes/` |
| `memory-schema` | Picoschema 模式管理：推断、创建、校验、漂移检测 | `~/.agents/skills/memory-schema/` |

---

## Codex Skills

| Skill | 功能简介 | 仓库 / 来源 | 本地路径 |
|-------|----------|-------------|----------|
| `skill-installer` | 从 curated 列表或 GitHub 仓库安装 Codex Skills | [openai/skills](https://github.com/openai/skills) | `~/.codex/skills/.system/skill-installer/` |
| `skill-creator` | 创建或更新 Codex Skill 的指南 | [openai/skills](https://github.com/openai/skills) | `~/.codex/skills/.system/skill-creator/` |
| `plugin-creator` | 脚手架化 Codex 插件目录与 marketplace 条目 | Codex 内置 | `~/.codex/skills/.system/plugin-creator/` |
| `openai-docs` | 查询 OpenAI 官方文档与模型选型建议 | [OpenAI Docs](https://platform.openai.com/docs) | `~/.codex/skills/.system/openai-docs/` |
| `imagegen` | AI 生成/编辑位图图像（照片、插画、mockup 等） | Codex 内置 | `~/.codex/skills/.system/imagegen/` |
| `legacy-codebase-mapper` | 遗留代码库测绘：入口、架构、数据流、迁移风险 | 本地自定义 | `~/.codex/skills/legacy-codebase-mapper/` |
| `paper-framework-figure-studio-pro` | 科研论文框架图设计与生成（方法图、架构图、流程图等） | 本地自定义（research-paper-figure-skill-factory v2.0.5） | `~/.codex/skills/paper-framework-figure-studio-pro/` |

---

## 快速选用

| 场景 | 推荐 Skill |
|------|------------|
| 新功能开发（完整流程） | `superpowers-workflow` |
| 只要计划 / checklist | `create-plan` |
| 陌生代码库上手 | `understand` → `understand-onboard` |
| PR 变更影响分析 | `understand-diff` |
| 看护 PR 直至可合并 | `babysit` |
| 代码安全审查 | `review-security` |
| 写 PRD / 做竞品分析 | `prd-development` / `competitive-analysis` |
| 程序化调用 Cursor Agent | `sdk` |
| 创建自定义 Skill | `create-skill` |

---

## 相关链接

- 本项目 Rules 索引：[INDEX.md](./INDEX.md)
- 开源 Rule 资源：[research/RULES-INDEX.md](./research/RULES-INDEX.md)
- Superpowers 文档：[obra-superpowers.mintlify.app](https://obra-superpowers.mintlify.app/)
- Understand Anything：[github.com/Lum1104/Understand-Anything](https://github.com/Lum1104/Understand-Anything)
- OpenAI Skills 仓库：[github.com/openai/skills](https://github.com/openai/skills)
