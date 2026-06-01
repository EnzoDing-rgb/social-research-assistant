---
name: social-research-assistant
description: 社科研究全流程 AI 助手。编排 GPT Researcher + Academic Research Skills + OpenSpec + Ralph Loop + Goal Workflow 为统一研究工作流。不造轮子，只做编排。
---

# Social Research Assistant

社科研究全流程 AI 助手。**不造新工具——编排现有最佳开源项目为一套研究工作流。**

> 站在 201K+ Stars 的肩膀上。一键安装，五工具齐备。

---

## 首次使用：检查依赖

启动研究前，先确认依赖工具是否就绪。如果缺失，Agent 会提示你运行：

```bash
bash setup.sh
```

这个脚本自动安装全部 5 个依赖。不需要手动一个个装。

---

## 工具箱（全自动安装）

| 工具 | 研究阶段 | Stars |
|------|---------|-------|
| **OpenSpec** | 定标准 — Spec-Driven 研究设计 | 46K+ |
| **GPT Researcher** | 搜文献 — 多源并行搜索 + 自动报告 | 26.6K+ |
| **Academic Research Skills** | 验质量 — 引用审计 + 多 Agent 交叉评审 | 14.7K+ |
| **Ralph Loop** | 自主迭代 — 不通过就换策略重来 | 官方 |
| **Goal Workflow** | 端到端 — /prd → /goal → /review-it → /ship | npx |

---

## 工作流

```
/spec → /research → /review → /revise → /ship
  │         │          │         │         │
  │         │          │         │         └─ Goal Workflow: 交付
  │         │          │         └─ Ralph Loop: 自主迭代修订
  │         │          └─ ARS: 多 Agent 交叉评审 + 引用审计
  │         └─ GPT Researcher: 多源并行搜索
  └─ OpenSpec: Spec-Driven 研究规格定义
```

---

## Phase 1: /spec — 定标准（OpenSpec）

研究开始前，先定义"什么叫做好了"。

**操作：**
```
/spec "你的研究问题"
```

**产出：** 研究规格说明书 — 研究问题 + 纳入/排除标准 + 质量门禁

**设计哲学：** OpenSpec 的 Delta Specs 机制——只写你这次要研究的东西，不重写全局。归档时自动合并到研究规格库。46K+ Stars 验证过的 Spec-Driven 模式。

---

## Phase 2: /research — 搜文献（GPT Researcher）

GPT Researcher 的 Planner → Executors → Publisher 架构。

```
研究问题 → Planner（拆解子问题）→ Executors×N（并行搜索）→ Publisher（汇总报告）
```

多个 Agent 独立搜索不同数据源，不共享中间结果——防止偏见传播。

**操作：**
```
/research "根据 spec.md 执行文献搜索"
```

**产出：** 带完整引用列表的结构化报告，每条标注来源类型。

---

## Phase 3: /review — 验质量（Academic Research Skills）

ARS 提供学术级质量保证。

**引用审计：** DOI 真伪 → 标题/作者匹配 → 论点忠实度检查
**交叉评审：** 3 Reviewer + 1 Devil's Advocate 独立打分
**防谄媚：** DA 退让必须有证据（Concession Threshold Protocol）

**关键数据：** 3 轮审核后独立审计仍发现 31% 的引用有问题。

**操作：**
```
/review  # 对搜索结果执行交叉评审
```

---

## Phase 4: /revise — 自主迭代（Ralph Loop）

评审不通过？Ralph Loop 自动换策略重来。最多 3 轮，Stop Hook 防死循环。

**操作：**
```
/revise  # 根据评审意见自主修订
```

---

## Phase 5: /ship — 交付（Goal Workflow）

四个命令串成闭环：`/prd` → `/goal` → `/review-it` → `/ship`

**操作：**
```
/ship  # 生成最终研究报告 + 验证追溯矩阵
```

---

## 概念来源

| 概念 | 工具 | 来源 |
|------|------|------|
| Spec-Driven | OpenSpec | 鸟窝 §03 |
| 多 Agent 交叉验证 | GPT Researcher + ARS | 鸟窝 §07 |
| Ralph Loop | ralph-wiggum | 鸟窝 §04 |
| Goal Workflow | goal-workflow | 鸟窝 §08 |
| Devil's Advocate | ARS v3.0 | ARS |
| Triangulation | 社科方法论经典 | Denzin 1978 |

---

## 适用/不适用

**适用：** 文献综述、系统综述、研究计划自检、投稿前完整性审计、灰色文献搜集

**不适用：** 原创理论建构、高度敏感的定性研究、替代人工同行评审
