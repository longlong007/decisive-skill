# Thinking Strategically Reference (English)

Source: Avinash K. Dixit & Barry J. Nalebuff, *Thinking Strategically: The Competitive Edge in Business, Politics, and Everyday Life*. **Read only the section for selected concepts** — do not read end-to-end.

Each entry: Source/Background → Definition → Formulas/Diagrams → When to apply → When not → Classic cases/counter-examples → Common misconceptions.

## Index

| Concept | Section | Game type |
|---------|---------|-----------|
| [Essence of strategic thinking](#essence-of-strategic-thinking) | Core | All |
| [Rule 1: Look ahead, reason back](#rule-1-look-ahead-reason-back) | Core | Sequential |
| [Mixed motives](#mixed-motives) | Core | All |
| [Prisoner's Dilemma](#prisoners-dilemma) | Core | Simultaneous/Repeated |
| [Rule 2: Dominant strategy](#rule-2-dominant-strategy) | Tools | Simultaneous |
| [Rule 3: Dominated strategy](#rule-3-dominated-strategy) | Tools | Simultaneous |
| [Rule 4: Nash equilibrium](#rule-4-nash-equilibrium) | Tools | Simultaneous |
| [Game tree & backward induction](#game-tree--backward-induction) | Tools | Sequential |
| [Payoff matrix & best response](#payoff-matrix--best-response) | Tools | Simultaneous |
| [Repeated games & Tit-for-Tat](#repeated-games--tit-for-tat) | Strategy | Repeated |
| [Strategic moves](#strategic-moves) | Strategy | Structure change |
| [Credible commitments](#credible-commitments) | Strategy | Commitment/threat |
| [Mixed strategy](#mixed-strategy) | Strategy | Simultaneous |
| [Brinkmanship](#brinkmanship) | Applications | Risk threats |
| [Cooperation & coordination](#cooperation--coordination) | Applications | Multi-party |
| [Voting strategy](#voting-strategy) | Applications | Collective choice |
| [Bargaining](#bargaining) | Applications | Division |
| [Incentive design](#incentive-design) | Applications | Mechanisms |

---

## Core Ideas

### Essence of strategic thinking

**Source/Background**: Game theory formalizes **strategic interdependence**—your outcome depends on others' purposeful choices while they reason about you. Applies across business, politics, parenting, and international relations.

**Definition**: The art of outdoing an opponent in interactive decisions while standing in their shoes to predict their best responses.

**Formulas/Diagrams**:

```
Three elements: Players → Moves → Payoffs
Strategic interdependence: U_i = f(a_i, a_{-i})
```

**When to apply**: Pricing, negotiation, voting, arms policy—any setting where your best move depends on others' moves.

**When not**: Pure personal preference with no interactive payoffs; random environments without strategic actors; mechanical optimization with no opponent.

**Classic cases/counter-examples**:
- Case: Adjacent gas stations setting prices while watching each other
- Counter: Choosing what to wear alone—no strategic interdependence

**Common misconceptions**:
- Optimizing only for yourself without simulating the opponent
- Equating "strategic" with "complicated"—simple dominant strategies often suffice

**Book anchor**: "Strategic thinking is the art of outdoing an adversary, knowing that the adversary is trying to do the same to you."

---

### Rule 1: Look ahead, reason back

**Source/Background**: The book's first rule; for all **sequential** games. Unlike a decision tree, a game tree requires multiple perspectives (you + opponent).

**Definition**: Forecast where your initial move will ultimately lead, then infer your best current choice (backward induction).

**Formulas/Diagrams**:

```
Game tree (simplified):

        [You: enter/exit]
       /               \
  [Rival: fight/deal]   [terminal payoffs]
   /           \
[terminal]  [terminal]

Steps: terminal nodes → best response at each node → roll back to root
```

**When to apply**: Chess endgames, sequential bargaining, product launch timing, litigation strategy.

**When not**: Strict simultaneous moves with no observability—use payoff matrix + equilibrium.

**Classic cases/counter-examples**:
- Case: Go endgame—reason from terminal position to current move
- Counter: Backward induction on a misspecified tree—garbage in, garbage out

**Common misconceptions**:
- Looking only one step ahead instead of to the game end
- Marking only your nodes as optimal, not the opponent's nodes from **their** view

---

### Mixed motives

**Source/Background**: Core insight—most real games are neither pure zero-sum nor pure cooperation.

**Definition**: Players face both conflict and shared interests—e.g., labor talks disagree on wages but both fear a strike.

**Formulas/Diagrams**:

```
Pure conflict (zero-sum):  u_1 + u_2 = 0
Pure cooperation:          aligned goals, coordination suffices
Mixed motives:             conflict on some dimensions + alignment on others (default)
```

**When to apply**: Business partnerships, diplomacy, team resource allocation, regulator-regulated relations.

**When not**: Strict zero-sum scoring; fully aligned teams with no resource tension.

**Classic cases/counter-examples**:
- Case: OPEC—compete for share yet jointly want high oil prices
- Counter: Modeling labor talks as pure zero-sum—misses mutual loss avoidance

**Common misconceptions**:
- Friend-or-foe binary framing
- Ignoring cooperative dimensions and missing Pareto improvements

---

### Prisoner's Dilemma

**Source/Background**: The book's central paradox; individual rationality → collective inefficiency. Repeated games, commitments, and punishment address this structure.

**Definition**: Each player has a **dominant strategy** to defect, yet mutual cooperation yields higher total payoffs; equilibrium is Pareto-dominated.

**Formulas/Diagrams**:

```
              Opponent cooperate   Opponent defect
You cooperate      (3,3)              (0,5)
You defect         (5,0)              (1,1)

→ (Defect, Defect) = Nash equilibrium; (Cooperate, Cooperate) Pareto superior
```

**When to apply**: Price wars, commons tragedy, arms races, free-riding, one-shot quality shirking.

**When not**: Effective repeated play with detection + punishment; enforceable contracts; pure coordination games.

**Classic cases/counter-examples**:
- Case: Duopoly price war—cutting price dominates, both profits fall
- Counter: Repeat procurement with observable quality and cutoff—one-shot PD logic fails

**Common misconceptions**:
- "Rational people should cooperate" in **one-shot** PD—defection is the rational equilibrium
- Calling any conflict a PD without verifying dominant defection structure

**Book anchor**: "Each player follows a dominant strategy, yet both end up worse off than if they had cooperated."

---

## Basic Tools

### Rule 2: Dominant strategy

**Source/Background**: Action Rule 2—first step in simultaneous games.

**Definition**: A strategy that yields higher payoff than every other **of your own** strategies, regardless of what the opponent does.

**Formulas/Diagrams**:

```
Row-dominance check: if Row A > Row B in every column → A dominates

Rule: play dominant strategy; expect opponent's dominant strategy if they have one
```

**When to apply**: Clear "always pick X" decisions; scan matrix before deeper equilibrium work.

**When not**: No dominant strategy (common); games requiring mixed strategies.

**Classic cases/counter-examples**:
- Case: Truthful bidding is dominant in second-price sealed-bid (Vickrey) auctions
- Counter: "Better than the opponent" ≠ dominant—dominance is vs **your other strategies**

**Common misconceptions**:
- Dominant ≠ better than opponent's strategy
- Dominant ≠ max-min—only needs to beat your alternatives in every column

---

### Rule 3: Dominated strategy

**Source/Background**: When no dominance exists, shrink the game by elimination.

**Definition**: Strategy D is always worse than strategy S regardless of opponent action; rational players never play D.

**Formulas/Diagrams**:

```
Iterated elimination:
1. Find dominated strategies → delete
2. Repeat on reduced game
3. If new dominance appears → Rule 2
```

**When to apply**: At least one side has ≥3 strategies; large matrices needing simplification.

**When not**: Continuous strategy spaces; no strict domination.

**Classic cases/counter-examples**:
- Case: Three-strategy voting game—"vote for worst" may be dominated
- Counter: Assuming opponent plays dominated strategy after elimination—violates rationality

**Common misconceptions**:
- One-round elimination only—iterate until no further elimination
- Confusing weak vs strict domination

---

### Rule 4: Nash equilibrium

**Source/Background**: John Nash; breaks the infinite "I think that you think…" loop.

**Definition**: Each player's strategy is a **best response** to others'; no one wants to deviate unilaterally.

**Formulas/Diagrams**:

```
(a_1*, a_2*) is Nash equilibrium ⟺
∀i: u_i(a_i*, a_{-i}*) ≥ u_i(a_i, a_{-i}*)  ∀a_i

Method: mark best responses → cells where all are best responses = equilibria
```

**When to apply**: Simultaneous pricing, advertising, tech choices—mutual guessing.

**When not**: Sequential information—use game trees; multiple equilibria need coordination/refinement.

**Classic cases/counter-examples**:
- Case: PD (Defect, Defect); Battle of Sexes has two equilibria
- Counter: Treating non-equilibrium profiles as stable—failed unilateral deviation check

**Common misconceptions**:
- Nash ≠ social optimum (PD equilibrium is inefficient)
- Assuming unique equilibrium—many games have several

---

### Game tree & backward induction

**Source/Background**: Standard tool for sequential games; multi-perspective unlike single-agent decision trees.

**Definition**: Tree of move order; infer optimal choices by backward induction from terminals.

**Formulas/Diagrams**: See [Rule 1](#rule-1-look-ahead-reason-back).

**When to apply**: Stackelberg leader-follower, sequential entry, multi-round bargaining.

**When not**: Simultaneous symmetric moves—use matrix.

**Classic cases/counter-examples**:
- Case: Market entry—incumbent threatens price war; entrant reasons backward on entry
- Counter: Ignoring information sets in incomplete information—needs subgame perfection

**Common misconceptions**:
- Using decision tree (one player) instead of game tree (many)
- Labeling opponent nodes with what **you** want, not their optimum

---

### Payoff matrix & best response

**Source/Background**: Visualization base for simultaneous games.

**Definition**: **Payoff matrix** lists strategy profiles and payoffs; **best response** is your highest-payoff move given opponent's strategy.

**Formulas/Diagrams**:

```
              Opponent: L    Opponent: R
You: U         (a,b)         (c,d)
You: D         (e,f)         (g,h)

If opponent plays L: compare your U vs D payoffs → higher is BR
```

**When to apply**: Two-dimensional strategy spaces; quick visual dominance/equilibrium checks.

**When not**: Continuous or high-dimensional strategy spaces without discretization.

**Classic cases/counter-examples**:
- Case: "Cover" method—one row entirely above another → row dominance
- Counter: Three+ players need higher-dimensional representation

**Common misconceptions**:
- Confusing payoff levels with ordinal rankings
- Swapping row vs column player roles

---

## Core Strategies

### Repeated games & Tit-for-Tat

**Source/Background**: Primary path out of PD; Axelrod's tournament validated Tit-for-Tat.

**Definition**: **Repeated games**—ongoing relationships make future loss discipline current defection; **Tit-for-Tat**—Clarity, Niceness, Provocability, Forgivingness.

**Formulas/Diagrams**:

```
Cooperation intuition:
discounted future cooperation gains > one-shot defection gain

Tit-for-Tat principles:
Clarity | Niceness (never defect first) | Provocability ( retaliate immediately) | Forgivingness (don't hold grudges)

Law of increasing transparency: cooperation on visible dimensions; competition shifts to hidden ones
```

**When to apply**: Long-term suppliers, repeat customers, ongoing teams, relations without known terminal date.

**When not**: **Finitely** repeated games with known end—backward unraveling; cheating undetectable; punishment not credible.

**Classic cases/counter-examples**:
- Case: TFT won Axelrod's tournament
- Counter: Last round of finitely repeated game—no future punishment, cooperation unravels backward

**Common misconceptions**:
- Repetition always yields cooperation—needs detection + punishment + uncertain horizon
- TFT universally optimal—noisy environments may over-punish

**Book anchor**: "If there is no tomorrow, today's promises cannot be retracted."

---

### Strategic moves

**Source/Background**: Change others' expectations to change behavior; preemptive in nature.

**Definition**:
- **Unconditional move**: unilaterally lock choice; convert simultaneous to sequential; first-mover advantage
- **Threat**: punish if opponent disobeys (changes response rule)
- **Promise**: reward if opponent complies (changes response rule)

**Formulas/Diagrams**:

```
Threat/Promise vs Warning/Assurance:

Warning/Assurance = inform what you would do anyway (information)
Threat/Promise = deliberately deviate from future natural optimum to manipulate opponent (credibility issue)

Threats/promises require future self-harming action → credibility problem
```

**When to apply**: Pre-negotiation commitments, entry deterrence, credible policy, contract design.

**When not**: Cheap talk with no cost; opponent cannot observe or verify.

**Classic cases/counter-examples**:
- Case: Burning bridges makes retreat impossible
- Counter: "If you raise prices I'll suicide-price"—if reneging is ex-post optimal, not credible

**Common misconceptions**:
- Treating warnings as threats without changing payoffs
- Extreme threats the opponent knows you won't execute

---

### Credible commitments

**Source/Background**: The book's **Eightfold Path**; incredible commitments void strategic moves.

**Definition**: Alter payoffs, reputation, or contracts so **keeping the commitment is self-interested** or **breaking it is very costly**.

**Formulas/Diagrams** — **Eightfold Path**:

| Path | Mechanism |
|------|-----------|
| Burn bridges | Remove retreat |
| Outsource control | Third party executes |
| Reputation capital | Breach cost > one-shot gain |
| Contract + bond | Economic penalty |
| Small steps | Split large promise |
| Team decision | Collective irreversibility |
| Standard operating procedure | Embed in process |
| No tomorrow | Final-stage irrevocability |

**When to apply**: Irreversible investment, M&A closing, policy credibility, military alliances.

**When not**: Cheap reneging; reputation worthless (one-shot anonymous play).

**Classic cases/counter-examples**:
- Case: Cortés scuttling ships
- Counter: International treaties without enforcement—no credible punishment

**Common misconceptions**:
- Verbal promise equals credible commitment
- Ignoring conversion of threat → warning by making execution self-optimal

---

### Mixed strategy

**Source/Background**: Predictable patterns get exploited; true randomization required.

**Definition**: Randomize across actions with specified probabilities so opponent **cannot predict** any single move; optimal mix makes opponent **indifferent** across responses.

**Formulas/Diagrams**:

```
Mixed strategy σ = (p_1, p_2, ...), Σp_i = 1

Optimum: opponent's payoffs from each pure response equal (indifference)

❌ Fixed alternation (predictable)
✅ True randomization (unpredictable)
```

**When to apply**: Tennis serves, promotion timing, tax audit frequency, military surprise—match vs mismatch games.

**When not**: Dominant pure strategy exists; pure coordination; predictability is the goal.

**Classic cases/counter-examples**:
- Case: Penalty kick random direction
- Counter: Fixed 50-50 alternation—pattern detectable

**Common misconceptions**:
- Mixed = arbitrary—requires indifference calculation
- Random = irrational—mixed strategies can be equilibrium

---

## Application Domains

### Brinkmanship

**Source/Background**: Thomas Schelling; classic framework for nuclear deterrence and crisis diplomacy.

**Definition**: Deliberately create **partially uncontrollable** recognizable risk so the situation "slightly slips out of control," forcing concession—probabilistic not deterministic threat.

**Formulas/Diagrams**:

```
Brinkmanship ≠ deterministic extreme threat (often incredible)
            = controlled slippery slope: risk rises gradually

Success: tunable risk | stepwise escalation | partial loss of control | clear exit
```

**When to apply**: Crisis bargaining, labor brinkmanship, regulatory tightening, commercial deadline pressure.

**When not**: Risk uncontrollable and unacceptable to you; opponent has no exit; one-shot cheap talk.

**Classic cases/counter-examples**:
- Case: Cuban Missile Crisis—controlled risk and communication
- Counter: "Surrender or nuclear war"—too extreme to be credible

**Common misconceptions**:
- Brinkmanship = bluff without real risk mechanism
- Risk too large—you also cannot accept the outcome

**Book anchor** (Schelling): "The deliberate creation of a recognizable risk of mutual harm."

---

### Cooperation & coordination

**Source/Background**: Cooperation defeats defection; coordination picks among multiple equilibria.

**Definition**:
- **Cooperation**: overcome PD-like temptation → repetition + punishment
- **Coordination**: select same equilibrium among many → **focal point**, convention, communication

**Formulas/Diagrams**:

```
Coordination (Battle of Sexes): multiple Nash equilibria—must pick the same one
Focal point: salient choice without communication—culture, convention, obviousness

Accordion effect: small reasonable steps → cumulative outcome bad for all (voting trap)
→ Rule 1: foresee endpoint from step one
```

**When to apply**: Industry standards, traffic rules, treaties, format wars, meeting times.

**When not**: Pure PD without coordination equilibrium—solve cooperation first.

**Classic cases/counter-examples**:
- Case: "Meet in New York"—Times Square as focal point
- Counter: No shared culture for focal point—coordination fails

**Common misconceptions**:
- Conflating cooperation with coordination—different tools
- Ignoring accordion effect cumulative trap

---

### Voting strategy

**Source/Background**: Democratic ideals vs strategic manipulation; Arrow's impossibility.

**Definition**: Strategic issues in aggregating preferences—cycles, agenda manipulation, strategic voting.

**Formulas/Diagrams**:

```
Voting cycle: A ≻ B ≻ C ≻ A → no stable winner; order determines outcome

Median voter theorem (1D): candidates converge to median
Multi-D: median vanishes → manipulation space grows

Strategic voting: vote for viable candidate vs favorite
```

**When to apply**: Boards, shareholder votes, elections, agenda-setting power.

**When not**: Two-person decisions; sincere voting is equilibrium special cases.

**Classic cases/counter-examples**:
- Case: Agenda manipulation changes Borda-like outcomes
- Counter: "My vote doesn't matter"—small individual impact, large cumulative effect

**Common misconceptions**:
- A "perfect" voting system exists (Arrow denies)
- Sincere voting is always optimal

**Book anchor**: "Power in voting can be weakness, and weakness can be power."

---

### Bargaining

**Source/Background**: Dividing the pie; rule-setting begins before formal talks.

**Definition**: Splitting surplus; **patience** and **outside options** set bargaining power.

**Formulas/Diagrams**:

```
Four elements:
1. Patience / waiting cost — more patient party gets larger share
2. "Hurts you more than me" — shift outside options
3. Rule-setting power — framing advantage
4. Multi-issue bundling — trade preference intensities

Infinite horizon intuition: limit shares ∝ relative patience (Rubinstein-type)
50:50 often equilibrium with symmetric patience
```

**When to apply**: Salary, M&A, alliances, treaties—any bilateral/multilateral division.

**When not**: Perfect competition pricing; no surplus to divide.

**Classic cases/counter-examples**:
- Case: First offer anchors the frame
- Counter: Ignoring outside option—misjudging BATNA

**Common misconceptions**:
- Bargaining is only about "fairness"—also patience and commitment game
- Single offer without subsequent rounds—misses sequential structure

---

### Incentive design

**Source/Background**: Mechanism design—align self-interest with social goals.

**Definition**: Tournaments, auctions, punishment, property rights, competition as institutional design.

**Formulas/Diagrams**:

```
Themes:
· Performance-incentive tradeoff (tournaments, relative rank)
· Internalize externalities (JVs, profit sharing)
· Vickrey auction: second price → truthful bid dominant
· Winner's curse: common-value auctions → winner often over-optimistic → shade bid down
· Punishment clarity: cheaters must predict consequences accurately
```

**When to apply**: Promotion, procurement auctions, JV governance, bequests, regulatory penalties.

**When not**: Effort fully observable and contractible—simple contracts suffice.

**Classic cases/counter-examples**:
- Case: Vickrey auction incentivizes truthful bids
- Counter: Offshore lease common-value auction—winner's curse overpayment

**Common misconceptions**:
- Confusing absolute vs relative performance incentives
- Ignoring innocent bystanders in collective punishment

---

## Problem → Tool chain

| Signal | Suggested concepts (2–4) |
|--------|--------------------------|
| First vs second mover | Rule 1, game tree, strategic moves |
| Simultaneous pricing/ads | Payoff matrix, Rules 2–4, PD |
| Long-term relationship | Repeated games, Tit-for-Tat, detection+punishment |
| Empty threats | Credible commitments, Eightfold Path, brinkmanship |
| Predictable pattern exploited | Mixed strategy |
| Which equilibrium | Cooperation & coordination, focal point |
| Board/shareholder vote | Voting strategy, agenda manipulation |
| Split surplus/contract | Bargaining, patience, outside options |
| Auction/promotion | Incentive design, Vickrey, winner's curse |

---

## Boundaries vs WRAP / Model Thinker

| Framework | Core question |
|-----------|---------------|
| **Thinking Strategically** | Interactive payoffs, opponent modeling, equilibrium & commitment |
| **WRAP** | Personal important choices, cognitive biases |
| **Model Thinker** | Multi-model understanding of complex systems |

Use this skill for strategic interaction; WRAP for personal choice; Model Thinker for systemic emergence/distribution/spread.
