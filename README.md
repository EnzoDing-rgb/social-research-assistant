# Research Assistant

Claude Code 科研全流程 AI 助手。迭代环架构：研究设计 → 文献搜索 → 实验设计 → 图表 & 结构 → 同行评审 → 路由修订 → 交付。

内置质量关卡、弱点路由表、跨模型交叉验证。

## 安装

```bash
bash setup.sh
```

安装 ARS + Ralph Loop。OpenSpec 可选。

## 技能文件

[research-skills.md](./research-skills.md) — 核心技能指南。包含完整工作流指令、子技能路由表、质量管理关卡、跨模型交叉验证策略。

## 示例

| 项目 | 说明 |
|------|------|
| [examples/world-model/](./examples/world-model/) | 世界模型综述 — 14 页，39 篇引用，李飞飞三分类框架 |
| [examples/tech-hiring/](./examples/tech-hiring/) | AI 替代与创造：中国技术招聘市场结构性变化（2023–2026） |

## 工具链

| 工具 | 用途 |
|------|------|
| Academic Research Skills (27.4K ⭐) | 文献搜索 + 同行评审 + 引用审计 |
| Ralph Loop | 定向路由修订 |
| OpenSpec（可选） | 研究设计 |

## 架构

```
研究设计 → 文献搜索 → 实验设计 → 图表 & 结构 → 同行评审 → 路由修订 → 交付
   ↑           ↑           ↑            ↑           │
   └───────────┴───────────┴────────────┴───────────┘
                    弱点路由表（定向修复，非盲目重试）
```

灵感来源：陈德里 DeliAutoResearch（DeepSeek, 2026）。
