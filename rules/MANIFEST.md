# Rules 文件清单

> 每个规则文件均标注参考来源、原始仓库地址及主要功能说明

---

## 📁 rules/shared/ — 跨平台通用规则

| 文件 | 主要功能 | 来源仓库 | 原始地址 |
|------|----------|----------|----------|
| `commit.mdc` | 标准化 Git 提交消息（Conventional Commits + emoji 格式） | steipete/agent-rules | https://github.com/steipete/agent-rules/blob/main/project-rules/commit.mdc |
| `bug-fix.mdc` | 结构化 Bug 修复流程（问题识别 → 根因分析 → 修复 → 预防） | steipete/agent-rules | https://github.com/steipete/agent-rules/blob/main/project-rules/bug-fix.mdc |
| `check.mdc` | 代码质量与安全全面检查，支持多语言静态分析 | steipete/agent-rules | https://github.com/steipete/agent-rules/blob/main/project-rules/check.mdc |
| `five.mdc` | 五问法（5 Whys）根本原因分析方法，深度理解问题根因 | steipete/agent-rules | https://github.com/steipete/agent-rules/blob/main/project-rules/five.mdc |
| `mermaid.mdc` | 自动生成 Mermaid 架构图和流程图（graph/flowchart/sequence） | steipete/agent-rules | https://github.com/steipete/agent-rules/blob/main/project-rules/mermaid.mdc |
| `pr-review.mdc` | 多角度 Pull Request 审查规范（代码/安全/性能/文档） | steipete/agent-rules | https://github.com/steipete/agent-rules/blob/main/project-rules/pr-review.mdc |
| `add-to-changelog.mdc` | 自动维护项目 CHANGELOG，遵循 Keep a Changelog 规范 | steipete/agent-rules | https://github.com/steipete/agent-rules/blob/main/project-rules/add-to-changelog.mdc |
| `clean.mdc` | 全代码库格式化修复（Python/JavaScript 等多语言） | steipete/agent-rules | https://github.com/steipete/agent-rules/blob/main/project-rules/clean.mdc |
| `context-prime.mdc` | 上下文加载优化指南，帮助 AI 快速理解项目全貌 | steipete/agent-rules | https://github.com/steipete/agent-rules/blob/main/project-rules/context-prime.mdc |
| `create-docs.mdc` | 文档创建规范（README / API / 架构图 / Mermaid 图表） | steipete/agent-rules | https://github.com/steipete/agent-rules/blob/main/project-rules/create-docs.mdc |
| `update-docs.mdc` | 文档更新规范，保持代码与文档同步一致 | steipete/agent-rules | https://github.com/steipete/agent-rules/blob/main/project-rules/update-docs.mdc |

---

## 📁 rules/cursor/ — Cursor 专属规则

### 通用基础层

| 文件 | 主要功能 | 来源仓库 | 原始地址 |
|------|----------|----------|----------|
| `core.mdc` | 项目通用规则核心层（始终生效） | flyeric0212/cursor-rules | https://github.com/flyeric0212/cursor-rules/blob/main/base/core.mdc |
| `general.mdc` | 通用编程规范（命名/注释/格式化） | flyeric0212/cursor-rules | https://github.com/flyeric0212/cursor-rules/blob/main/base/general.mdc |
| `project-structure.mdc` | 项目代码结构与文件组织规范 | flyeric0212/cursor-rules | https://github.com/flyeric0212/cursor-rules/blob/main/base/project-structure.mdc |
| `tech-stack.mdc` | 技术栈定义与官方文档链接 | flyeric0212/cursor-rules | https://github.com/flyeric0212/cursor-rules/blob/main/base/tech-stack.mdc |

### 框架层

| 文件 | 主要功能 | 来源仓库 | 原始地址 |
|------|----------|----------|----------|
| `react.mdc` | React 应用开发规范（组件/hooks/状态管理） | flyeric0212/cursor-rules | https://github.com/flyeric0212/cursor-rules/blob/main/frameworks/react.mdc |
| `vuejs.mdc` | Vue.js 应用开发规范（Composition API/选项式） | flyeric0212/cursor-rules | https://github.com/flyeric0212/cursor-rules/blob/main/frameworks/vuejs.mdc |
| `nextjs.mdc` | Next.js 全栈框架规范（App Router/SSR/API Routes） | flyeric0212/cursor-rules | https://github.com/flyeric0212/cursor-rules/blob/main/frameworks/nextjs.mdc |
| `tailwind.mdc` | Tailwind CSS 样式规范（原子化 CSS 实践） | flyeric0212/cursor-rules | https://github.com/flyeric0212/cursor-rules/blob/main/frameworks/tailwind.mdc |
| `django.mdc` | Django Python Web 框架规范（MTV 架构） | flyeric0212/cursor-rules | https://github.com/flyeric0212/cursor-rules/blob/main/frameworks/django.mdc |
| `fastapi.mdc` | FastAPI Python 现代 Web 框架规范（异步/Pydantic） | flyeric0212/cursor-rules | https://github.com/flyeric0212/cursor-rules/blob/main/frameworks/fastapi.mdc |
| `swiftui.mdc` | SwiftUI Apple 平台 UI 框架规范 | flyeric0212/cursor-rules | https://github.com/flyeric0212/cursor-rules/blob/main/frameworks/swiftui.mdc |

### 语言层

| 文件 | 主要功能 | 来源仓库 | 原始地址 |
|------|----------|----------|----------|
| `python.mdc` | Python 编程规范（PEP 8 / 类型注解 / 异步） | flyeric0212/cursor-rules | https://github.com/flyeric0212/cursor-rules/blob/main/languages/python.mdc |
| `typescript.mdc` | TypeScript 编程规范（类型安全 / 接口 / 泛型） | flyeric0212/cursor-rules | https://github.com/flyeric0212/cursor-rules/blob/main/languages/typescript.mdc |
| `java.mdc` | Java 编程规范（OOP / 异常处理 / Maven） | flyeric0212/cursor-rules | https://github.com/flyeric0212/cursor-rules/blob/main/languages/java.mdc |
| `golang.mdc` | Go 编程规范（并发 / 错误处理 / GOPATH） | flyeric0212/cursor-rules | https://github.com/flyeric0212/cursor-rules/blob/main/languages/golang.mdc |

### 其他

| 文件 | 主要功能 | 来源仓库 | 原始地址 |
|------|----------|----------|----------|
| `git.mdc` | Git 使用规范（提交规范 / 分支策略 / Rebase） | flyeric0212/cursor-rules | https://github.com/flyeric0212/cursor-rules/blob/main/other/git.mdc |
| `document.mdc` | 项目文档编写规范（README / API 文档 / 注释） | flyeric0212/cursor-rules | https://github.com/flyeric0212/cursor-rules/blob/main/other/document.mdc |

---

## 📁 rules/claude-code/ — Claude Code 安全规则

### 核心安全层

| 文件 | 主要功能 | 来源仓库 | 原始地址 |
|------|----------|----------|----------|
| `owasp-2025.md` | OWASP Top 10 2025 安全标准（Web 安全基础） | TikiTribe/claude-secure-coding-rules | https://github.com/TikiTribe/claude-secure-coding-rules/blob/main/rules/_core/owasp-2025.md |
| `agent-security.md` | Agentic AI 自主行为安全（工具调用 / 多步骤任务） | TikiTribe/claude-secure-coding-rules | https://github.com/TikiTribe/claude-secure-coding-rules/blob/main/rules/_core/agent-security.md |
| `ai-security.md` | AI 系统通用安全规范（数据隐私 / 对抗攻击） | TikiTribe/claude-secure-coding-rules | https://github.com/TikiTribe/claude-secure-coding-rules/blob/main/rules/_core/ai-security.md |
| `mcp-security.md` | MCP（Model Context Protocol）安全规范 | TikiTribe/claude-secure-coding-rules | https://github.com/TikiTribe/claude-secure-coding-rules/blob/main/rules/_core/mcp-security.md |
| `rag-security.md` | RAG 系统安全（向量检索 / 注入攻击 / 数据泄露） | TikiTribe/claude-secure-coding-rules | https://github.com/TikiTribe/claude-secure-coding-rules/blob/main/rules/_core/rag-security.md |
| `graph-database-security.md` | 图数据库安全（Neo4j / 权限控制 / 查询注入） | TikiTribe/claude-secure-coding-rules | https://github.com/TikiTribe/claude-secure-coding-rules/blob/main/rules/_core/graph-database-security.md |

### 语言安全

| 文件 | 主要功能 | 来源仓库 | 原始地址 |
|------|----------|----------|----------|
| `python-security.md` | Python 安全编码规范（依赖安全 / 输入验证） | TikiTribe/claude-secure-coding-rules | https://github.com/TikiTribe/claude-secure-coding-rules/blob/main/rules/languages/python/CLAUDE.md |
| `typescript-security.md` | TypeScript 安全编码规范（类型安全 / XSS 防护） | TikiTribe/claude-secure-coding-rules | https://github.com/TikiTribe/claude-secure-coding-rules/blob/main/rules/languages/typescript/CLAUDE.md |
| `javascript-security.md` | JavaScript 安全编码规范（前端安全 / 加密） | TikiTribe/claude-secure-coding-rules | https://github.com/TikiTribe/claude-secure-coding-rules/blob/main/rules/languages/javascript/CLAUDE.md |

### 框架安全

| 文件 | 主要功能 | 来源仓库 | 原始地址 |
|------|----------|----------|----------|
| `react-security.md` | React 安全编码规范（XSS / CSRF / 状态管理） | TikiTribe/claude-secure-coding-rules | https://github.com/TikiTribe/claude-secure-coding-rules/blob/main/rules/frontend/react/CLAUDE.md |
| `nextjs-security.md` | Next.js 安全编码规范（SSR / API Routes / 认证） | TikiTribe/claude-secure-coding-rules | https://github.com/TikiTribe/claude-secure-coding-rules/blob/main/rules/frontend/nextjs/CLAUDE.md |
| `fastapi-security.md` | FastAPI 安全编码规范（依赖注入 / 认证 / CORS） | TikiTribe/claude-secure-coding-rules | https://github.com/TikiTribe/claude-secure-coding-rules/blob/main/rules/backend/fastapi/CLAUDE.md |

### 基础设施安全

| 文件 | 主要功能 | 来源仓库 | 原始地址 |
|------|----------|----------|----------|
| `cicd-security.md` | CI/CD 安全规范（GitHub Actions / GitLab CI） | TikiTribe/claude-secure-coding-rules | https://github.com/TikiTribe/claude-secure-coding-rules/blob/main/rules/cicd/_core/cicd-security.md |
| `container-security.md` | 容器安全规范（Docker / K8s / Helm） | TikiTribe/claude-secure-coding-rules | https://github.com/TikiTribe/claude-secure-coding-rules/blob/main/rules/containers/_core/container-security.md |
| `iac-security.md` | IaC 安全规范（Terraform / Pulumi / 基础设施审计） | TikiTribe/claude-secure-coding-rules | https://github.com/TikiTribe/claude-secure-coding-rules/blob/main/rules/iac/_core/iac-security.md |

---

## 📁 rules/devin/ — Devin 增强规则（Cursor/Windsurf 通用）

| 文件 | 主要功能 | 来源仓库 | 原始地址 |
|------|----------|----------|----------|
| `cursorrules.md` | 智能任务规划与自我进化（规划 → 执行 → 校准 → 积累循环） | grapeot/devin.cursorrules | https://github.com/grapeot/devin.cursorrules/blob/master/.cursorrules |
| `scratchpad.md` | 持久化 Scratchpad，记录任务进度、经验教训和学习积累 | grapeot/devin.cursorrules | https://github.com/grapeot/devin.cursorrules/blob/master/scratchpad.md |

---

_创建时间：2026-06-16_
_最后更新：2026-06-16_
_来源：基于 research/RULES-INDEX.md 中调研的开源项目_