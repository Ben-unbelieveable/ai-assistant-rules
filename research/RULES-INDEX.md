# 🔥 开源 AI 助手 Rules 资源索引

> 调研日期：2026-06-16 | 来源：GitHub / CSDN / 掘金 / 技术博客

---

## 一、⭐ 核心标杆项目（跨平台 / 高影响力）

### 1. steipete / agent-rules
**⭐ 标杆级跨平台规则引擎**

| 项目 | 说明 |
|------|------|
| **GitHub** | https://github.com/steipete/agent-rules |
| **定位** | AI 编码助手规则引擎与知识库系统 |
| **格式** | `.mdc`（Markdown with Configuration） |
| **平台** | Cursor ✅ / Claude Code ✅ / 其他 ⚠️ 手动适配 |
| **Stars** | 较高（社区活跃） |

**核心规则文件：**

| 文件 | 功能 |
|------|------|
| `commit.mdc` | 标准化 Git 提交消息（Conventional Commits + emoji） |
| `check.mdc` | 代码质量检查与静态分析 |
| `bug-fix.mdc` | 结构化 Bug 修复流程 |
| `five.mdc` | 五问法根本原因分析（5 Whys） |
| `mermaid.mdc` | Mermaid 图表自动生成 |
| `modern-swift.mdc` | Swift/SwiftUI 最佳实践 |
| `add-to-changelog.mdc` | 变更日志维护 |

**`.mdc` Frontmatter 规范（关键创新）：**
```yaml
---
description: "规则描述"
globs: ["**/*.js"]           # 应用文件模式
alwaysApply: false           # 是否始终应用
priority: high              # 优先级：high / normal / low
language: javascript        # 目标语言
---
```

**导入方式：**
```markdown
@import "https://raw.githubusercontent.com/steipete/agent-rules/main/project-rules/commit.mdc"
```

**提取规范：**
- ✅ Frontmatter 元数据层（description / globs / alwaysApply / priority / language）
- ✅ Conventional Commits 标准化提交格式
- ✅ 五问法（5 Whys）根因分析流程
- ✅ Bug 修复四步法：问题识别 → 根因分析 → 修复实施 → 预防措施
- ✅ Mermaid 架构图集成
- ✅ 条件规则应用（`{{#if isSwiftProject}}`）

---

### 2. PatrickJS / awesome-cursorrules
**⭐ 最大的 .cursorrules 文件集合**

| 项目 | 说明 |
|------|------|
| **GitHub** | https://github.com/PatrickJS/awesome-cursorrules |
| **定位** | 社区驱动的 .cursorrules 文件资源库 |
| **格式** | `.cursorrules` / `.mdc` |
| **平台** | Cursor ✅ |
| **Stars** | 社区活跃 |

**覆盖范围：**
- 前端框架：React / Angular / Vue / Next.js
- 后端/全栈：Node.js / Python / Go / Laravel
- 移动开发：React Native / SwiftUI / Flutter
- CSS 框架：Tailwind CSS / Bootstrap
- 更多持续收录中

**提取规范：**
- 按技术栈分类的规则隔离
- 项目级 AI 行为定制（代码风格、技术栈约束）
- 安全与性能规范

---

### 3. cursor.directory
**⭐ 官方推荐规则目录**

| 项目 | 说明 |
|------|------|
| **官网** | https://cursor.directory/ |
| **GitHub** | https://github.com/pontusab/cursor.directory |
| **定位** | 专为 Cursor 设计的开源资源库 |
| **格式** | `.cursorrules` |
| **平台** | Cursor ✅ |
| **覆盖** | 30+ 主流语言和框架 |

**支持技术栈（部分）：**
Python / FastAPI / Django / Next.js / TypeScript / Node.js / React / Vue / Tailwind CSS / Go / Rust / Java / Kotlin / Swift 等

**提取规范：**
- 预置配置文件 + 提示词库
- AI 规则优化方案
- 多语言开发场景支持

---

## 二、🇨🇳 中文社区热门项目

### 4. Mr-chen-05 / rules-2.1-optimized
**企业级 AI 助手规则体系（中文优化版）**

| 项目 | 说明 |
|------|------|
| **GitHub** | https://github.com/Mr-chen-05/rules-2.1-optimized |
| **定位** | 基于 agent-rules 优化扩展，专为中国开发者打造 |
| **平台** | Augment ✅ / Cursor ✅ / Claude Code ✅ / 更多 |
| **目录** | `global-rules/` / `docs/` / `mcp-scripts/` / `install-scripts/` |

**核心特点：**
- 企业级规则体系
- 中文注释和文档
- 安装脚本，开箱即用

**提取规范：**
- 企业级开发规范模板
- 跨工具统一配置方案

---

### 5. flyeric0212 / cursor-rules
**Cursor Rules 规则汇总（中文）**

| 项目 | 说明 |
|------|------|
| **GitHub** | https://github.com/flyeric0212/cursor-rules |
| **定位** | 整理和收集来自不同项目的 Cursor 规则文件 |
| **Stars** | 持续更新 |

**目录结构（分层设计）：**

```
base/           # 基础规则
demo/           # 示例
frameworks/     # 框架规则（React / Vue.js / Next.js / Tailwind CSS 等）
languages/      # 编程语言规则（Python / Java / TypeScript / Go / C++ / Kotlin / C# 等）
other/          # 其他规则
```

**三层规则架构：**

| 层级 | 规则 | 说明 |
|------|------|------|
| **通用规则层** | `core.mdc` / `tech-stack.mdc` / `project-structure.mdc` | 始终生效，提供基础规范 |
| **编程语言层** | `python.mdc` / `java.mdc` / `typescript.mdc` 等 | 根据文件扩展名自动应用 |
| **框架层** | `react.mdc` / `vuejs.mdc` / `nextjs.mdc` 等 | 根据上下文自动判断 |

**提取规范：**
- 分层规则架构（通用 → 语言 → 框架）
- 技术栈定义与官方文档链接
- 项目结构和文件组织规范

---

## 三、📋 Claude Code 专用规则

### 6. Lance-He / claude-md-rules
**Claude Code 多语言编程规则文件集合**

| 项目 | 说明 |
|------|------|
| **GitHub** | https://github.com/Lance-He/claude-md-rules |
| **定位** | 为 Claude Code 提供多语言编程规则文件（CLAUDE.md） |
| **目录** | `C/` / `Frontend/` / `Java/` 等 |

**提取规范：**
- 按语言分类的 CLAUDE.md 规则
- 通用开发标准（GENERAL_DEVELOPMENT_STANDARDS.md）

---

### 7. TikiTribe / claude-secure-coding-rules
**⭐ 安全编码规则（高价值细分领域）**

| 项目 | 说明 |
|------|------|
| **GitHub** | https://github.com/TikiTribe/claude-secure-coding-rules |
| **定位** | 为 Claude Code 提供安全编码规则 |
| **Stars** | 活跃维护（65 Commits） |

**覆盖范围：**
- Web 应用安全
- AI/ML 系统安全
- Agentic AI 安全
- 前端框架安全
- 51+ RAG 工具安全
- IaC（Terraform/Pulumi）
- 容器（Docker/K8s/Helm）
- CI/CD（GitHub Actions/GitLab CI）

**三种执行模式：**
| 模式 | 说明 |
|------|------|
| **Strict** | 强制执行，违规代码拒绝生成 |
| **Warning** | 警告模式，提示安全风险 |
| **Advisory** | 建议模式，提供最佳实践 |

**提取规范：**
- 安全优先的代码生成规范
- 分层执行模式（Strict / Warning / Advisory）
- 涵盖 OWASP Top 10 / 数据加密 / 输入验证 / 依赖安全

---

## 四、🚀 Cursor 增强规则

### 8. grapeot / devin.cursorrules（原始版）
**将 Cursor 提升为接近 Devin 的体验**

| 项目 | 说明 |
|------|------|
| **GitHub** | https://github.com/grapeot/devin.cursorrules |
| **定位** | 智能流程规划与自我进化能力扩展 |
| **平台** | Cursor ✅ / Windsurf ✅ |

**核心亮点：**
- 智能任务规划与自我校准
- 扩展工具集成（网页浏览、搜索、AI 分析）
- 自动化执行流程
- 持续积累个人使用场景的规则

**提取规范：**
- 任务规划 → 执行 → 校准 → 添加 的循环流程
- Scratchpad 持久化记录
- 自动化自我优化机制

---

### 9. WhiteCrow / devin.cursorrules
**devin.cursorrules 的另一个活跃分支**

| 项目 | 说明 |
|------|------|
| **GitHub** | https://github.com/WhiteCrow/devin.cursorrules |
| **特点** | 包含 `.devcontainer` / `.windsurfrules` / `scratchpad.md` |

---

## 五、📖 各平台原生规则文件

### 10. 各平台规则文件对照表

| 平台 | 规则文件名 | 位置 | 说明 |
|------|----------|------|------|
| **Claude Code** | `CLAUDE.md` | 项目根目录 或 `~/.claude/` | 主规则文件，支持 `@import` |
| **Cursor** | `.cursorrules` 或 `.mdc` | 项目根目录 `~/.cursor/rules/` | 支持分层目录 |
| **OpenClaw** | `SOUL.md` / `AGENTS.md` / `*.md` | workspace 目录 | Agent 规则体系 |
| **Windsurf** | `.windsurfrules` | 项目根目录 | 与 Cursor 类似 |
| **Cline** | `.clinerules` | 项目根目录 | Cline 专用 |
| **GitHub Copilot** | `copilot.md` | 项目根目录 | GitHub Copilot 规则 |

---

## 六、📐 提取的通用 Rule 规范

### 规范分类汇总

#### A. 代码质量类
| 规范 | 来源 | 说明 |
|------|------|------|
| Conventional Commits | steipete/agent-rules | 提交消息标准化（feat/fix/docs/style/refactor/test/chore） |
| 代码审查清单 | steipete/agent-rules | 多语言静态分析 |
| 安全编码规则 | TikiTribe/claude-secure-coding-rules | OWASP Top 10 / 加密 / 输入验证 |

#### B. 开发流程类
| 规范 | 来源 | 说明 |
|------|------|------|
| Bug 修复四步法 | steipete/agent-rules | 问题识别 → 根因分析 → 修复实施 → 预防措施 |
| 五问法（5 Whys） | steipete/agent-rules | 根因分析方法 |
| 任务规划循环 | grapeot/devin.cursorrules | 规划 → 执行 → 校准 → 添加 |

#### C. 文档与可视化类
| 规范 | 来源 | 说明 |
|------|------|------|
| Mermaid 图表 | steipete/agent-rules | 架构图、流程图自动生成 |
| 变更日志维护 | steipete/agent-rules | CHANGELOG 自动更新 |
| README 生成 | 各项目通用 | 项目文档标准结构 |

#### D. 规则格式类
| 规范 | 来源 | 说明 |
|------|------|------|
| Frontmatter 元数据 | steipete/agent-rules | description / globs / alwaysApply / priority / language |
| 分层规则架构 | flyeric0212/cursor-rules | 通用层 → 语言层 → 框架层 |
| 条件规则应用 | steipete/agent-rules | `{{#if isSwiftProject}}` 类条件判断 |

---

## 七、📚 参考资料来源

| 来源 | 类型 | URL |
|------|------|-----|
| steipete/agent-rules | GitHub | https://github.com/steipete/agent-rules |
| PatrickJS/awesome-cursorrules | GitHub | https://github.com/PatrickJS/awesome-cursorrules |
| cursor.directory | GitHub | https://github.com/pontusab/cursor.directory |
| Mr-chen-05/rules-2.1-optimized | GitHub | https://github.com/Mr-chen-05/rules-2.1-optimized |
| flyeric0212/cursor-rules | GitHub | https://github.com/flyeric0212/cursor-rules |
| Lance-He/claude-md-rules | GitHub | https://github.com/Lance-He/claude-md-rules |
| TikiTribe/claude-secure-coding-rules | GitHub | https://github.com/TikiTribe/claude-secure-coding-rules |
| grapeot/devin.cursorrules | GitHub | https://github.com/grapeot/devin.cursorrules |
| WhiteCrow/devin.cursorrules | GitHub | https://github.com/WhiteCrow/devin.cursorrules |
| Agent Rules CSDN 博客 | CSDN | https://blog.csdn.net/j8267643/article/details/151721233 |
| CSDN .cursorrules 收集博客 | CSDN | https://blog.csdn.net/j8267643/article/details/147687247 |
| 掘金 Awesome CursorRules | 掘金 | https://juejin.cn/post/7480350360964448293 |
| 掘金 Devin.cursorrules | 掘金 | https://juejin.cn/post/7482668843921866762 |
| CSDN 通用 AI 编程规则 | CSDN | https://blog.csdn.net/LinqiOTO/article/details/160045860 |
| CSDN Cursor Rules 实战 | CSDN | https://blog.csdn.net/u012743772/article/details/161179078 |

---

_最后更新：2026-06-16_
_维护者：Ben-unbelieveable_