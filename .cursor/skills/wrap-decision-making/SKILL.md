---
name: wrap-decision-making
description: Guides structured decision-making using the WRAP framework from Chip and Dan Heath's Decisive (决断力). Use when the user faces an important choice, feels stuck between options, shows narrow framing, confirmation bias, short-term emotion, or overconfidence, or asks for WRAP, Decisive, premortem, tripwire, 决断力, 拓宽选择, 现实检验, or better decision-making help. Responds in the user's language (English or 中文).
---

# WRAP Decision Framework

Based on *Decisive: How to Make Better Choices in Life and Work* by Chip Heath & Dan Heath. Source: [Heath Brothers WRAP one-pager](https://heathbrothers.com/wp-content/uploads/resources/The_WRAP_Process_one_pager.pdf).

## Language

**Match the user's language.** Use localized section headings — never mix English headings in 中文 responses.

| User language | Read also |
|---------------|-----------|
| English (default) | [techniques.en.md](techniques.en.md) |
| 中文 | [reference.zh.md](reference.zh.md) + [techniques.zh.md](techniques.zh.md) |

Use Chinese book terminology in 中文 responses (e.g. 思维狭隘, 证实倾向, 绊网, 书档, 事前验尸). Keep WRAP as the acronym in both languages.

## When to Apply

Use WRAP as the **sole primary framework** (do not stack with other decision models) when:

- The user faces an **important** work, career, or life decision
- Multiple biases appear together: narrow framing, confirmation bias, short-term emotion, overconfidence
- The user mentions WRAP, Decisive, 决断力, widening options, disconfirming evidence, psychological distance, premortem, or tripwire

**Not applicable**: trivial reversible choices → use **WRAP Lite** even if user invokes `/wrap-decision-making`.

## Pre-Flight (before W → R → A → P)

Run in order. Stop early when a gate triggers.

### 1. Non-Negotiables Check

Scan for hard constraints that **eliminate options before widening**:

| Category | Examples |
|----------|----------|
| Health & safety | Toxic exposure, physical harm, untreated medical risk |
| Legal & compliance | Illegal activity, contract breach, regulatory violation |
| Family & living | Cannot work from home, caregiving duties, visa/residency limits |
| Financial survival | Cannot afford option without confirmed income |
| Ethics | Values the user would not trade for any benefit |

If an option violates a non-negotiable (confirmed or highly likely): **exclude it**; do not list it as a viable alternative. State which constraint removed it.

If constraint status is **unknown** → trigger Information Gate (do not guess that an option is safe).

### 2. Information Gate

**Trigger** when any **critical constraint** needed for a defensible recommendation is unknown — e.g. current situation vs. stated options mismatch, budget ceiling, health exposure, reversibility, timeline, who else is affected.

**When triggered**:

- Output **Gate template only** (see below)
- Ask **1–3 questions**, **one at a time** in conversation; combine in a single message only if ≤3 and tightly related
- **Forbidden**: Recommendation, Next Action, WRAP Analysis, proposed options that assume unknown facts
- After user answers → re-run pre-flight, then proceed to Full or Lite

**Do not trigger** when missing info is nice-to-have but a reasonable Lite pass is still useful (e.g. lunch preference).

## Four Villains → Technique Selection

Diagnose dominant bias(es). Pick **one primary** for W/R technique binding. Cap outputs per step:

| Villain | W (max) | R (max) | Primary technique |
|---------|---------|---------|-------------------|
| Narrow framing | +1 new option, 1 baseline | — | Vanishing options test **or** multitracking |
| Confirmation bias | — | 1 assumption, 1 disconfirm | Disconfirming question **or** ooch |
| Short-term emotion | — | — | A: one distance question (friend / 10-10-10 / core priority) |
| Overconfidence | — | 1 base-rate question | Zoom out **+** premortem + 1 tripwire in P |

Secondary biases: address in analysis text only; do not add more options or questions beyond caps.

Execute W → R → A → P in order. Mark each step: `applied` / `satisfied by existing info` / `skipped (not applicable)`.

### W — Widen Your Options

**Goal**: Escape whether-or-not framing (Think AND, not OR).

**Baseline options** (name at most **one** that applies): do nothing / delay / combine / small experiment.

**Constraints**:

- AI-proposed options: label `AI suggestion — pending confirmation`; **max 1** new option unless user asked for brainstorming
- Never propose options that fail non-negotiables or depend on unverified assumptions

### R — Reality-Test Your Assumptions

**Goal**: One disconfirming item that could **change** the decision.

**Constraints**: Do not fabricate external facts. Prices, stats, policies, market rates → suffix `(pending verification)` / `（待核实）`, or convert to a user verification action.

### A — Attain Distance Before Deciding

**Goal**: Reduce short-term emotion distortion.

**Trigger only when** emotion or external pressure may obscure core goals. Otherwise mark `skipped`. Use **one** distance technique.

### P — Prepare to Be Wrong

**Goal**: Observable tripwires, not vague flexibility.

**Required**: premortem (1 failure scenario + 1 early signal) + **1 tripwire** (stop or reopen). Preparade only when upside is plausible.

## Execution Constraints

1. Ask **one** question at a time across turns; ≤3 core questions before first Recommendation.
2. WRAP steps are a **background checklist** — output length governed by templates below, not step count.
3. Do not re-ask derivable information. **Multi-turn**: delta updates only (see Multi-Turn Rules).
4. Recommendations state assumptions and uncertainty; never guarantee outcomes.
5. Final decision returns to the user (accept / adjust / reject) — do not decide for them.

## Mode Selection

| Mode | When |
|------|------|
| **Gate** | Critical constraints unknown |
| **Lite** | Trivial/reversible choice; or low stakes + clear preference path |
| **Full** | Important decision + enough confirmed constraints |
| **Delta** | Round 2+ in same decision thread |

**Hard limits**: Gate ≤15 lines · Lite ≤20 lines · Full ≤80 lines · Delta ≤40 lines.

## Multi-Turn Rules

When the user adds facts in a follow-up (same decision thread):

1. **Rewrite Decision Statement** if framing changed (e.g. user already has an office; question is stay vs. leave).
2. Output **Delta template** — do **not** repeat unchanged W/R/A/P bullets.
3. Revise only affected steps + Recommendation/Next Action if direction changed.
4. New questions: only those unlocked by the update; still max 1 per message.

## Output Templates

### Gate (information insufficient)

```markdown
## Decision Statement
[Provisional one sentence — note what's uncertain]

## Pending Clarification
Critical constraints are unclear. Need your input before recommending:

1. [Most important question]
2. [Optional second]
3. [Optional third]

_No recommendation until the above is confirmed._
```

### WRAP Lite (≤20 lines)

**Include**: Decision Statement · 1-line bias note · W (+1 option OR 1 baseline) · R (1 disconfirm) · A (1 line, or skip) · P (1 tripwire) · Direction (1 sentence) · Next Action (1 step).

**Omit**: Full WRAP Analysis headers · status fields · Bias checkbox block · Reasons list · Key tradeoff / Critical assumption / Uncertainty blocks · Preparade · Reopen condition (unless essential).

```markdown
## Decision Statement
[One sentence]

[One-line bias note, e.g. "Narrow framing — treating this as binary."]

**W**: [Current options + at most 1 AI suggestion — pending confirmation]
**R**: [One disconfirming question or micro-experiment]
**A**: [One distance line, or "Skipped — facts-driven, low emotion."]
**P**: [One tripwire]

**Direction**: [One sentence; user decides]
**Next**: [One action within 48h]
```

### WRAP Full (≤80 lines)

**Include all sections below.** Per-step caps from technique table still apply. Keep prose tight.

**Omit**: Repeating technique catalog · long option lists · unverified numbers without `（待核实）` / `(pending verification)`.

```markdown
## Decision Statement
[One sentence]

## Bias Diagnosis
[Active villains — brief; no checkbox block required]

## Non-Negotiables
[Confirmed constraints that filter options, or "None identified"]

## WRAP Analysis

### W — Widen Your Options
- Status: [applied / satisfied / skipped]
- Options: [user-confirmed + ≤1 AI suggestion — pending confirmation]
- Baseline: [one applicable]

### R — Reality-Test Your Assumptions
- Status: [applied / satisfied / skipped]
- Key assumption: [one]
- Disconfirm: [one question or experiment]

### A — Attain Distance Before Deciding
- Status: [applied / satisfied / skipped]
- [Core priority or one distance conclusion — only if triggered]

### P — Prepare to Be Wrong
- Status: [applied / satisfied / skipped]
- Premortem: [one scenario + one signal]
- Tripwire: [one observable trigger]

## Recommendation
**Direction**: [clear recommendation]
**Reasons** (max 3):
1. ...
2. ...
3. ...

**Key tradeoff**: [...]
**Critical assumption**: [...]
**Uncertainty**: [high/medium/low + reason]

## Next Action
- **Action**: [48h executable step]
- **Success criteria**: [...]
- **Stop condition**: [...]
- **Reopen condition**: [...]
```

### Delta (round 2+, ≤40 lines)

```markdown
## Decision Statement (updated)
[Reframed decision]

## What Changed
- [New fact and why it matters]

## Updated Analysis
[Only affected W/R/A/P items]

## Recommendation
[Revised direction, or "unchanged" + why]

## Next Action
[Revised step if needed]
```

## External Facts Rule

Any **price, statistic, rate, policy, or third-party claim** not provided by the user:

- Append `（待核实）` / `(pending verification)`, **or**
- Replace with: "Verify: [specific action user can take in 48h]"

Never present unverified numbers as grounds for Recommendation.

## Quick Examples

**Gate**: "Library or rent an office?" — unknown whether user can work from home → Gate only; ask where they work today and why they're considering a change.

**Lite**: "螺蛳粉 or 江西米粉 for lunch" → Lite template; 10/10/10 in one line; no full analysis.

**Full**: Job switch with known salary, industry, and timeline → Full template; R uses one base-rate verification action (待核实).

**Delta**: User reveals shared office with 3D-print fumes → rewrite statement; update W (exclude "home + library"); non-negotiable health filter; delta only.

## Additional Resources

- English techniques: [techniques.en.md](techniques.en.md)
- 中文流程与模板: [reference.zh.md](reference.zh.md)
- 中文技法: [techniques.zh.md](techniques.zh.md)
- Framework source: [Decisive](https://heathbrothers.com/books/decisive/) — Chip Heath & Dan Heath
