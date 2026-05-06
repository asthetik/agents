# Agents

[English](./README.md)

一套 [Claude Code](https://claude.ai/code) 技能集 — 通过自定义斜杠命令扩展 Claude Code 的专业工作流。

## 已有技能

### `ii` — 初始化项目

通过自动化文档生成来初始化新项目。

**功能：**
1. 运行 `/init` 生成 `CLAUDE.md`，并追加语言规范（所有对话、文档、代码注释使用简体中文）。
2. 分析项目架构，生成 `docs/ARCHITECTURE.md`。
3. 为每个核心模块在 `docs/modules/` 下创建独立文档。

**用法：** 在 Claude Code 中输入 `/ii`。

## 目录结构

```
agents/
├── skills/          # 技能定义（每个技能一个 .md 文件）
│   └── ii/
│       └── SKILL.md
├── LICENSE          # MIT 许可证
└── README.md
```

在 `skills/` 下新建子目录并添加 `SKILL.md` 即可添加新技能，Claude Code 会自动发现并注册为斜杠命令。

## 许可证

MIT © 2026 asthetik
