---
name: wrap-decision-making
description: Guides structured decision-making using the WRAP framework from Chip and Dan Heath's Decisive (决断力). Use when the user faces an important choice, feels stuck between options, shows narrow framing, confirmation bias, short-term emotion, or overconfidence, or asks for WRAP, Decisive, premortem, tripwire, 决断力, 拓宽选择, 现实检验, or better decision-making help. Responds in the user's language (English or 中文).
---

# WRAP Decision Framework

Based on *Decisive: How to Make Better Choices in Life and Work* by Chip Heath & Dan Heath. Source: [Heath Brothers WRAP one-pager](https://heathbrothers.com/wp-content/uploads/resources/The_WRAP_Process_one_pager.pdf).

## Language

**Match the user's language.**

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

**Not applicable**: missing facts that require minimum-evidence action first; trivial reversible choices (use reversibility/small-experiment framing instead).

## Four Villains of Decision Making

Diagnose which bias dominates — each maps to one WRAP step:

| Villain | Signal | Step |
|---------|--------|------|
| Narrow framing | Stuck in yes/no; ignores third paths | W |
| Confirmation bias | Collects only supporting evidence | R |
| Short-term emotion | Driven by present anxiety or excitement | A |
| Overconfidence | Assumes the future is predictable; no Plan B | P |

## WRAP Process

Execute W → R → A → P in order. Mark each step: `applied` / `satisfied by existing info` / `skipped (not applicable)`.

### W — Widen Your Options

**Goal**: Escape whether-or-not framing; consider multiple directions (Think AND, not OR).

**Baseline options** (retain at least one that applies):
- Do nothing (status quo)
- Delay the decision
- Combine options
- Small-scale experiment (ooch precursor)

**Techniques** (pick 1–2; see [techniques.en.md](techniques.en.md)):
- Find someone who already solved this problem
- Laddering: local bright spots → regional best practices → distant analogies
- Multitracking: pursue 2–3 options in parallel, not serial elimination
- Vanishing options test: "If none of the current options were available, what would you do?"

**Constraint**: AI-proposed options must be labeled "AI suggestion — pending confirmation."

### R — Reality-Test Your Assumptions

**Goal**: Actively seek **disconfirming** evidence that could change the decision.

**Techniques** (prioritize 1 disconfirming question or minimum experiment):
- Disconfirming questions: "What's the biggest problem with this option?"
- Zoom out: What are the base rates for similar decisions?
- Zoom in: What unique details in this case change the general pattern?
- Ooch: Replace prediction with a small experiment ("Why predict when you can know?")

**Constraint**: Do not fabricate external facts; when evidence is missing, generate user-executable verification actions.

### A — Attain Distance Before Deciding

**Goal**: Reduce distortion from short-term emotion; return to core priorities.

Trigger **one** distance question only when emotion or external pressure may obscure core goals:

- What would you tell your best friend to do?
- What would your successor do?
- 10/10/10: How will you feel in 10 minutes / 10 months / 10 years?
- Clarify core priorities: What does this decision truly need to protect?

### P — Prepare to Be Wrong

**Goal**: Accept uncertainty; prepare for bad and good outcomes; set re-evaluation triggers.

**Must land on observable conditions** — not vague "stay flexible":

- **Premortem**: Assume failure in 6–12 months; most likely causes? Early warning signals?
- **Preparade**: Assume unexpected success; what must be prepared in advance?
- **Tripwire**: What observable signal triggers re-evaluation or stop? (stop condition / reopen condition)

## Execution Constraints

1. Ask **one** necessary question at a time; at most **3** core guiding questions.
2. WRAP four steps run as a background checklist — no four long forms for the user.
3. Do not re-ask steps derivable from confirmed user information.
4. Recommendations must state assumptions and uncertainty; never guarantee outcomes.
5. Final decision returns to the user (accept / adjust / reject).

## WRAP Lite (time-constrained)

When a full pass is too heavy:

1. **W**: Add one more option (or find someone who solved this).
2. **R**: Call an expert for base rates, or ask one disconfirming question.
3. **A**: Which option best fits core values?
4. **P**: Bookend the future — 1 hour on what could go wrong/right; prepare for both.

## Output Template

```markdown
## Decision Statement
[One sentence describing the decision]

## Bias Diagnosis
- [ ] Narrow framing  [ ] Confirmation bias  [ ] Short-term emotion  [ ] Overconfidence
[Brief note on which biases are active]

## WRAP Analysis

### W — Widen Your Options
- Status: [applied / satisfied / skipped]
- Current options: [user-confirmed]
- New options (if any): [labeled AI suggestion — pending confirmation]
- Baseline options: [do nothing / delay / combine / small experiment]

### R — Reality-Test Your Assumptions
- Status: [applied / satisfied / skipped]
- Key assumptions: [list]
- Disconfirming evidence or experiment: [one item that could change the decision]

### A — Attain Distance Before Deciding
- Status: [applied / satisfied / skipped]
- Core priority: [long-term goal to protect]
- Distance perspective: [10/10/10 or friend/successor view conclusion]

### P — Prepare to Be Wrong
- Status: [applied / satisfied / skipped]
- Premortem: [failure scenario and warning signals]
- Preparade (if applicable): [unexpected-success scenario]
- Tripwire: [observable stop/reopen/re-evaluate trigger]

## Recommendation
**Direction**: [clear recommendation]
**Reasons** (max 3):
1. ...
2. ...
3. ...

**Key tradeoff**: [what you gain vs. give up]
**Critical assumption**: [if false, recommendation fails]
**Uncertainty**: [high/medium/low + reason]

## Next Action
- **Action**: [specific step executable within 48 hours]
- **Success criteria**: [how to know the action worked]
- **Stop condition**: [when to abandon this direction]
- **Reopen condition**: [when to reconsider rejected options]
```

## Quick Example

**Input**: "I'm considering leaving my job for a new company — 30% higher pay but a different industry."

**W**: Beyond leave/stay, propose "side project to test the new industry" and "re-evaluate in 6 months" → labeled AI suggestion.
**R**: "What percentage of people in that industry stay employed after 3 years?" "Can 2 weeks of informational interviews validate culture fit?"
**A**: 10/10/10 — if you regret this in 10 months, most likely because of what?
**P**: Tripwire — if core project delivery slips >2 weeks within 90 days due to the learning curve, trigger re-evaluation.

## Additional Resources

- English techniques: [techniques.en.md](techniques.en.md)
- 中文流程与模板: [reference.zh.md](reference.zh.md)
- 中文技法: [techniques.zh.md](techniques.zh.md)
- Framework source: [Decisive](https://heathbrothers.com/books/decisive/) — Chip Heath & Dan Heath
