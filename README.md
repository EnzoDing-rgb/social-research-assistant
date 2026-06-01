# Social Research Assistant

社科研究全流程 AI 助手。**不造新工具——编排现有最佳开源项目为一套研究工作流。**

> 站在 201K+ Stars 的肩膀上。一键安装，五工具齐备。

## 一键安装

```bash
# 1. 安装插件（Claude Code）
/plugin marketplace add enzoding/social-research-assistant
/plugin install social-research-assistant

# 2. 安装依赖工具（自动装全部）
bash setup.sh
```

**安装内容：**

| 工具 | 用途 | Stars |
|------|------|-------|
| [OpenSpec](https://github.com/Fission-AI/OpenSpec) | Spec-Driven 研究规格定义 | 46K+ |
| [GPT Researcher](https://github.com/assafelovic/gpt-researcher) | 自主深度搜索 + 自动报告 | 26.6K+ |
| [Academic Research Skills](https://github.com/Imbad0202/academic-research-skills) | 引用审计 + 多 Agent 评审 | 14.7K+ |
| [Ralph Loop](https://github.com/anthropics/ralph-wiggum) | 自主迭代——不通过就重来 | 官方 |
| [Goal Workflow](https://github.com/smallnest/goal-workflow) | 端到端闭环——/prd → /ship | npx |

## 快速开始

```bash
# 在 Claude Code 中输入研究问题
/spec "社交媒体对青少年心理健康的影响"
/research
/review
/revise
/ship
```

五个命令，一条流水线，从研究问题到验证报告。

## 工作流

```
/spec → /research → /review → /revise → /ship
 定标准    搜文献      验质量      自主迭代    交付
```

## 设计哲学

> You can outsource your thinking, but you cannot outsource your understanding.

**AI 干脏活：** 搜文献、验引用、交叉比对、迭代修订
**你做判断：** 定问题、选方法、写 "I argue that" 后面那句话

## 适用场景

- 文献综述 / 系统综述
- 研究计划质量检查
- 投稿前完整性审计
- 跨方法对比分析
- 灰色文献搜集

## License

MIT
