# AI Assistant Rules

跨平台 AI 助手规则库，管理 Claude Code / Cursor / OpenClaw 等通用规则，实现多平台同步更新迭代。

## 平台兼容

| 平台 | 状态 |
|------|------|
| Claude Code | ✅ |
| Cursor | ✅ |
| OpenClaw | ✅ |
| 其他 | 待扩展 |

## 目录结构

```
ai-assistant-rules/
├── README.md
├── LICENSE
├── rules/
│   ├── shared/          # 通用规则（所有平台适用）
│   ├── claude-code/     # Claude Code 专属
│   ├── cursor/          # Cursor 专属
│   └── openclaw/       # OpenClaw 专属
└── docs/
    └── PLATFORMS.md     # 平台差异说明
```

## 规则同步机制

通用规则放在 `rules/shared/`，各平台通过引用或软链方式接入。
平台专属规则放在对应目录，独立维护。

## 贡献指南

1. 通用规则优先写入 `rules/shared/`
2. 平台专属规则写入对应目录
3. 新增规则需标注适用平台
4. 更新时保持跨平台兼容性

## License

MIT