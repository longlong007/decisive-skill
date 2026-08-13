---
name: thinking-strategically
description: Guides strategic thinking using Dixit & Nalebuff's Thinking Strategically (策略性思考)—game theory for interactive decisions in business, politics, and daily life. Use when the user faces strategic interdependence, payoffs depend on others' choices, needs Nash equilibrium / prisoner's dilemma / credible commitment / brinkmanship / bargaining / voting strategy analysis, or mentions 策略性思考, 博弈论, 向前展望向后推理, 囚徒困境, 纳什均衡, 以牙还牙, 边缘政策, 可信承诺. Responds in the user's language (English or 中文).
---

# Thinking Strategically (策略性思考)

Based on *Thinking Strategically: The Competitive Edge in Business, Politics, and Everyday Life* by Avinash K. Dixit & Barry J. Nalebuff（《策略性思考》）。详见 [reference.zh.md](reference.zh.md) / [reference.en.md](reference.en.md)。

## Language

**Match the user's language.** Localized headings only.

| User language | Concept reference |
|---------------|-------------------|
| English | [reference.en.md](reference.en.md) |
| 中文 | [reference.zh.md](reference.zh.md) |

**Retrieval**: 用 reference 顶部索引选概念 → **只读对应小节**（来源/背景/定义/公式图示/适用/不适用/案例/误区）。勿通读 reference。

Keep **Nash Equilibrium**, **Prisoner's Dilemma**, **Tit-for-Tat**, **Brinkmanship** in both languages where standard.

## When to Apply

- Outcome depends on **others' purposeful choices** (strategic interdependence)
- Need to predict / influence / design in competitive or mixed-motive settings
- User mentions game theory, 博弈, 占优策略, 承诺, 威胁, 混合策略, 谈判, 投票策略, etc.

**Not primary**: pure personal preference choice without interdependence (use WRAP); pure statistical forecasting without strategic actors; trivial one-shot decisions with no payoff linkage.

**Vs WRAP / Model Thinker**: Thinking Strategically = **interactive payoffs & opponent modeling**; WRAP = personal option choice; Model Thinker = multi-model system understanding. Don't stack as competing primaries.

## Pre-Flight

### 1. Game Type Gate

| Type | Signal | Primary tool |
|------|--------|--------------|
| **Sequential** | moves in order, can observe prior moves | Game tree + backward induction (Rule 1) |
| **Simultaneous** | act at same time, mutual guessing | Payoff matrix + equilibrium (Rules 2–4) |
| **Repeated** | same players, ongoing relationship | Detection + punishment + Tit-for-Tat |
| **Mixed-motive** | both conflict and common interest | Don't assume pure zero-sum or pure cooperation |

Unclear → ask **one** question (sequential vs simultaneous? one-shot vs repeated?).

### 2. Information Gate

Critical unknowns (payoffs, outside options, commitment ability, detection of cheating, number of players, stakes) → Gate only; no fabricated equilibrium claims (`待核实` / `pending verification`).

### 3. Opponent Stance

Label per analysis: **Rational** (best response) · **Reputation-bound** · **Procedural / institutional** (SOP, brinkmanship). Mixed → note per branch.

## Workflow

Cap **2–4 concepts** (default **2–3**). Label: `applied` / `ruled out` / `pending data`.

### Step 1 — Map situation

Identify: Players · Moves · Payoffs · Sequential or simultaneous · One-shot or repeated · Pure conflict, cooperation, or **mixed-motive**.

### Step 2 — Select tools (Rules 1–4 order)

1. **Rule 1** (sequential): Look ahead, reason back → backward induction on game tree
2. **Rule 2**: Dominant strategy? → play it; expect opponent's dominant strategy
3. **Rule 3**: Dominated strategies? → eliminate; iterate
4. **Rule 4**: Nash equilibrium / best-response fixed point

For PD-like structures → reference: [重复博弈与以牙还牙](reference.zh.md#重复博弈与以牙还牙) / repeated games, [可信承诺](reference.zh.md#可信承诺) / credible commitments, [战略行动](reference.zh.md#战略行动) / strategic moves.

### Step 3 — Apply (per concept)

From reference, extract only selected sections:

- **Setup**: players, strategies, payoff structure (1–2 lines)
- **Implication** for user's move
- **Conditionality** · **Falsifier**
- Optional: **书中语** (verbatim anchor from reference)

No textbook dump. Include payoff matrix / tree sketch only when it changes the recommendation.

### Step 4 — Credibility & dynamics check

If threat, promise, or commitment involved → distinguish **威胁/承诺 vs 警告/保证**; apply Eightfold Path or flag credibility gap.

If cooperation needed → check detection + punishment; finite horizon trap.

### Step 5 — Synthesize

Conditional strategic recommendation · opponent's likely response · one next move or probe.

Final call stays with user.

## Constraints

1. Always model **both sides** — "put yourself in their shoes."
2. Mixed-motive is default; zero-sum and pure cooperation are special cases.
3. One clarifying question per turn (≤3 if Gate).
4. Multi-turn → **Delta** only.
5. Don't confuse dominant strategy with "better than opponent."

## Modes

| Mode | When | Limit |
|------|------|-------|
| **Gate** | Game type / payoffs unknown | ≤15 lines |
| **Lite** | Quick strategic read | ≤35 lines |
| **Full** | Complex interaction + enough context | ≤100 lines |
| **Delta** | Round 2+ | ≤40 lines |

### Gate

```markdown
## 博弈框架
[一句：谁、什么选择、为何相互依存]

## 待澄清
1. …

_确认前不做均衡推断。_
```

### Lite

```markdown
## 博弈框架
## 博弈类型
Sequential / Simultaneous · One-shot / Repeated

## 工具（2–3）
1. **[概念]**: 含义 · 对你意味着什么 · 失效条件
…

## 建议行动
```

### Full

```markdown
## 博弈框架
## 博弈类型 · 对手立场 · 混合动机诊断

## 分析
### 1. [概念]
- Setup · 公式/矩阵/树 · Implication · Conditionality · Falsifier

## 可信度 / 动态检验
## 综合建议
```

### Delta

```markdown
## 博弈框架（更新）
## 变化
## 更新分析
## 综合建议
```

## Quick Rule Reference

| Rule | Content |
|------|---------|
| **Rule 1** | Look ahead and reason back (backward induction) |
| **Rule 2** | If you have a dominant strategy, use it |
| **Rule 3** | Eliminate dominated strategies |
| **Rule 4** | Look for equilibrium (Nash) |

## Examples

- 价格战是否跟进 → Lite：同时行动矩阵 + 占优/均衡 + PD 结构
- 谈判谁先报价 → Full：顺序博弈 + 耐心/外部选项 + 规则制定权
- 如何维持供应商合作 → Full：重复博弈 + 检测/惩罚 + Tit-for-Tat 四原则

## Additional Resources

- Full concept library: [reference.zh.md](reference.zh.md) · [reference.en.md](reference.en.md)
- Personal life decisions without strategic interdependence → [wrap-decision-making](../wrap-decision-making/SKILL.md)
- System-level multi-model analysis → [model-thinker](../model-thinker/SKILL.md)
