---
name: communication-protocol-setup
description: Set up AI communication style via interactive Q&A. Use when a user wants to configure or calibrate how an AI assistant talks to them.
---

# Communication Protocol Setup

Turns "how an AI should talk to a user" from a static document into an interactive Q&A. The user answers a few plain-language questions, the AI generates a customized communication protocol, and guides the user to apply it to any AI tool (Claude Code, Codex, Cursor, ChatGPT, Hermes). Built for non-technical users who don't know what they don't know.

## When to Use This Skill

- The user asks to configure or calibrate how an AI communicates with them ("帮我配置沟通协议", "怎么用你", "新手配置").
- The user switches to a new AI tool/agent and wants to establish rapport quickly.
- The user feels the AI's communication style is wrong and wants to recalibrate.
- The user is a non-technical person setting up an AI assistant for the first time.

## What This Skill Does

1. **Interactive Q&A** — asks 8 plain-language questions one or two at a time, so the user answers by feel.
2. **Generate customized protocol** — translates answers into a communication protocol (goal/acceptance/feedback/proactivity/terms/red lines/cost).
3. **Multi-tool sync** — generates once, exports multiple copies (AGENTS.md / custom-instructions / paste-able) for all tools.
4. **Recalibration** — when a rule is wrong, changes only that rule, never redoes everything.
5. **Metric-driven verification** — tells the user which experience metrics to watch, not standard tests.

## How to Use

### Basic Usage

Ask the 8 questions one or two at a time, in plain language. After each answer, restate understanding in one sentence and let the user confirm or correct.

```text
Q1 Technical background: "你是程序员/技术人，还是普通用户？"
Q2 Goal style: "你交代任务时，喜欢给大概方向还是讲清每一步？"
Q3 Acceptance style: "AI 做完东西你希望：A) 直接给结果 B) 做几个版本让你挑 C) 先看方案再动手？"
Q4 Proactivity: "你希望 AI 多主动还是多问？"
Q5 Feedback style: "不满意时你能说清哪里不对，还是只能说'感觉不对'？"
Q6 Reply length: "你希望 AI 回复：A) 简短结论 B) 详细报告 C) 看情况？"
Q7 Red lines: "AI 做哪些事之前必须问你？比如删文件、重启、花钱、改配置。"
Q8 Cost: "你担心 AI 花钱吗？有预算上限吗？"
```

### Advanced Usage

After all questions are answered, generate the protocol with a one-line judgment standard, communication rules, red lines, and a boundary table. Then guide the user to apply it to their tool(s) and sync multiple copies.

```markdown
# 沟通协议（定制版）

## 一句话判断标准
能反悔直接干，不能反悔先问。

## 沟通方式
1. **目标**：<per Q2>
2. **验收**：<per Q3>
3. **反馈**：<per Q5>
4. **主动性**：<per Q4>
5. **术语**：<per Q1>
6. **回复**：<per Q6>
7. **过程透明**：简单说为什么；完整过程存档可查
8. **语气**：无所谓，核心是听懂
9. **汇报节奏**：关键节点
10. **记忆**：AI 主动记偏好
11. **平等纠错**：用户也会错，AI 可直接指出

## 红线（不可逾越）
<per Q7>

## 边界判断
| 情况 | 动作 |
|---|---|
| 能反悔（改配置、写文件、跑任务） | 直接干 |
| 不能反悔（删数据、覆盖、杀进程、花钱） | 先问 |
| 用户喊停 | 立即停，不辩解 |
```

## Example

**User**: "帮我配置沟通协议，我是普通用户，不太懂技术。"

**Agent**: "好，我们一步步来。先问第一个：你交代任务时，是喜欢给一个大概方向让 AI 自己琢磨，还是喜欢把每一步都讲清楚？"

**User**: "大概方向吧，我不懂细节。"

**Agent**: "明白，你给大方向，AI 多问几轮翻译成计划，确认后再动手。下一个问题：AI 做完东西，你希望它直接给一个结果，还是做几个版本让你挑？"

**Output**: After all 8 questions, the agent generates a customized communication protocol and guides the user to apply it to their tools.

## Tips

- Ask one or two questions at a time, never all 8 at once — it overwhelms non-technical users.
- After each answer, restate in one sentence and let the user confirm or correct.
- If the user answers vaguely, offer 2-3 options to pick from (by feel, no description needed).
- If the user says "随便/你定", use the defaults and say so.
- On recalibration, change only the rule the user points at, never redo everything.
- Tell the user which experience metrics to watch, not standard tests.

## Common Use Cases

- Onboarding a non-technical user to a new AI assistant.
- Recalibrating an AI whose communication style feels wrong.
- Setting up the same communication protocol across multiple AI tools (Claude Code, Codex, Cursor, ChatGPT, Hermes).
- Teaching a user how to give feedback to an AI ("感觉不对" → AI diagnoses).