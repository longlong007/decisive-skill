# Model Reference (English)

Source: Scott E. Page, *The Model Thinker*. **Read only the section for selected models** — do not read end-to-end.

Each entry: Definition → Background → Principle → How to use → When to apply → When not → Book anchor.

## Index

| Model | Ch | Primary REDCAPE |
|-------|-----|-----------------|
| [Many-model thinking](#many-model-thinking) | 1 | C, R |
| [REDCAPE](#redcape) | 2 | All |
| [Science of many models](#science-of-many-models) | 3 | P, R |
| [Modeling human actors](#modeling-human-actors) | 4 | Cross-cutting |
| [Normal distribution](#normal-distribution) | 5 | E, P |
| [Power-law](#power-law) | 6 | E, P |
| [Preferential attachment](#preferential-attachment) | 6 | E |
| [Linear models](#linear-models) | 7 | E, A, P |
| [Nonlinear models](#nonlinear-models) | 8 | E, R |
| [Value & power](#value--power) | 9 | R, D |
| [Networks](#networks) | 10 | E, P |
| [Broadcast](#broadcast) | 11 | P, E |
| [Diffusion](#diffusion) | 11 | P, E |
| [Bass model](#bass-model) | 11 | P |
| [SIR model](#sir-model) | 11 | P, A |
| [Entropy](#entropy) | 12 | E, R |
| [Random walk](#random-walk) | 13 | P, R |
| [Path dependence](#path-dependence) | 14 | E, R |
| [Local interaction](#local-interaction) | 15 | E, Explore |
| [Lyapunov functions](#lyapunov-functions) | 16 | R |
| [Markov models](#markov-models) | 17 | P, E |
| [Systems dynamics](#systems-dynamics) | 18 | E, D, A |
| [Threshold models](#threshold-models) | 19 | E, P |
| [Spatial competition](#spatial-competition) | 20 | D, E |
| [Hedonic competition](#hedonic-competition) | 20 | E, P |
| [Game theory](#game-theory) | 21 | R, A |
| [Cooperation](#cooperation) | 22 | E, D |
| [Collective action & commons](#collective-action--commons) | 23 | D, A |
| [Mechanism design](#mechanism-design) | 24 | D, A |
| [Signaling](#signaling) | 25 | E, R |
| [Learning models](#learning-models) | 26 | E, P |
| [Multi-armed bandit](#multi-armed-bandit) | 27 | A, P |
| [Rugged landscape](#rugged-landscape) | 28 | Explore, A |

---

## Foundations

### Many-model thinking

**Definition**: Understand complex phenomena via a **diverse ensemble** of formal, simplified models—not one master model.

**Background**: Data-rich era still needs structure; single-cause narratives (grit-only, capital-only) are incomplete. Munger / Aristotle multi-window metaphor.

**Principle**: Each model highlights different forces; overlaps weave richer understanding. All models wrong (Box); ensembles reduce blind spots. Wisdom hierarchy: data → information → knowledge → wisdom.

**How to use**: (1) Set REDCAPE purpose. (2) Pick 2–5 diverse models. (3) Apply → cross-check → conditional synthesis. (4) Never claim one equation explains society.

**When to apply**: Complex systems; explain/predict/design/explore; single-narrative blind spots.

**When not**: Fact lookup; option-choice-only (use WRAP); pure code without analysis.

**Book anchor**: "Many-model thinking produces wisdom through diverse logical frames."

---

### REDCAPE

**Definition**: Seven model purposes—Reason, Explain, Design, Communicate, Act, Predict, Explore.

**Background**: Schools emphasize explain; real world uses predict, design, act, explore.

**Principle**: Success criteria differ by purpose (interpretability vs prediction). Reason reveals **conditional** truth. Three build modes: embodiment, analogy, alternative reality.

**How to use**: (1) Lock one primary purpose. (2) Simpler models for R/E/C/Explore; higher fidelity OK for P/D/A but still ensemble. (3) Match build mode to task.

**When to apply**: Before any formal modeling—clarify what the model is **for**.

**When not**: Unspecified purpose + formula dumping.

**Book anchor**: "REDCAPE—the red cape—many-model power."

---

### Science of many models

**Definition**: Condorcet jury / diversity prediction theorems justify ensembles; independent accurate models are **limited** in number.

**Background**: Classification dimension caps useful models (~3–7, not 50); Google interviews, economist forecasts show diminishing returns.

**Principle**: Ensemble gains need signal + uncorrelated errors. Data dimension limits distinct partitions.

**How to use**: Prioritize diversity over count; drop near-duplicate partitions; cite "3 random economists beat 1 best" for prediction.

**When to apply**: Justifying multi-model; ensemble forecast/classification.

**When not**: Unlimited stacking without diversity check.

**Book anchor**: "In practice, 'many' may be closer to 5 than 50."

---

### Modeling human actors

**Definition**: How to model people—orgs: fixed rules, adaptive rules, or rational optimization.

**Background**: No universal behavior theory; need consistent frame to combine models.

**Principle**: Low stakes → fixed rules; feedback/imitation → learning; high stakes/experience → rational benchmark. Mixed stances OK in one ensemble if **labeled**.

**How to use**: Match stance to stakes and repetition; rational as benchmark/testable prediction, not default truth.

**When to apply**: Human/org decisions; incentives and information matter.

**When not**: Pure physical systems without agents.

**Book anchor**: "How we model people depends on context and purpose."

---

## Distributions & scale

### Normal distribution

**Definition**: Bell-shaped symmetric distribution; limit of sums/averages of independent random variables.

**Background**: Core modeling knowledge; contrast with power-law.

**Principle**: Central Limit Theorem; Six Sigma assumes additive errors.

**How to use**: Check independent small factors summing; use mean ± SD; **do not** extrapolate tail risk if power-law suspected.

**When to apply**: Independent increments; rare extremes; QC, sample means.

**When not**: Earthquakes, war deaths, book sales, wealth—often power-law; winner-take-most feedback.

**Book anchor**: "Add or average random variables → expect normal."

---

### Power-law

**Definition**: Long tail—many small events, few huge; probability inversely related to size.

**Background**: Cities, links, citations, shocks; vs normal drives risk framing.

**Principle**: Preferential attachment, self-organized criticality; exponent reflects volatility.

**How to use**: Log-scale/rank plots; manage extremes not just mean; compare insurance/buffer under normal vs power-law.

**When to apply**: Dependence, feedback, no hard cap, rich-get-richer.

**When not**: IID sums; binding caps; insufficient data to distinguish from lognormal.

**Book anchor**: "Without models, power-law is unexplained pattern."

---

### Preferential attachment

**Definition**: Arrivals join existing entity with probability ∝ size; prob p create new entity.

**Background**: Matthew effect—more leads to more.

**Principle**: Size → attraction → larger size → power-law tail.

**How to use**: Spot success-begets-success; estimate p and concentration; policy: antitrust, seeds, entry barriers.

**When to apply**: Open growth; reinforcement of advantage.

**When not**: Uniform random assignment; hard quotas blocking feedback.

**Book anchor**: "Matthew effect: more leads to more."

---

## Functional form

### Linear models

**Definition**: y = mx + b (possibly multivariate regression).

**Background**: Simplest, widest use; first-order approximations.

**Principle**: Slope = marginal effect; skill-luck decomposition guides "reward skill not luck."

**How to use**: Baseline regression; interpret sign/magnitude; upgrade if curvature/thresholds; avoid big-coefficient-only thinking.

**When to apply**: Local linearity; first-order causal/predictive analysis.

**When not**: Increasing/decreasing returns; thresholds; forever 10% growth extrapolation.

**Book anchor**: "Big-coefficient thinking kills innovation."

---

### Nonlinear models

**Definition**: Effects change with level—concave (diminishing), convex (increasing), thresholds.

**Background**: Linear is start; world is mostly nonlinear.

**Principle**: Concavity → diversity & risk aversion; convexity → risk-seeking & superlinear scale; classification via linear/nonlinear/trees/forests ensemble.

**How to use**: Classify marginal returns; concave → diversify; convex → watch runaway feedback.

**When to apply**: Diminishing utility; network effects; changing policy margins.

**When not**: Narrow range still linear and decisions stay in range.

**Book anchor**: "This is, after all, a nonlinear world."

---

### Value & power

**Definition**: Cooperative game metrics—last-on-the-bus (LOTB), Shapley value.

**Background**: Team output hard to split; seats ≠ voting power.

**Principle**: Shapley = average marginal contribution over join orders; axioms: null, symmetry, efficiency, additivity.

**How to use**: Define V(S); compute Shapley/LOTB; voting—separate seat share from swing power.

**When to apply**: Contribution splits, voting power, bargaining baselines.

**When not**: Undefined coalitions; pure zero-sum competition.

**Book anchor**: "20% seats may mean zero power in one vote, 1/3 in another."

---

## Networks & spread

### Networks

**Definition**: Nodes + edges; degree, path length, clustering, communities.

**Background**: Markets, supply chains, social, finance; embedding enriches any spread/game model.

**Principle**: Friendship paradox; weak ties, six degrees; structure affects diffusion, robustness, aggregation.

**How to use**: Map topology type; find hubs, clusters, bridges; overlay spread/cooperation on network.

**When to apply**: Who connects to whom matters; not well-mixed.

**When not**: Mass-action well-mixed sufficient.

**Book anchor**: "Networks almost always matter."

---

### Broadcast

**Definition**: Informed/uninformed; single source broadcasts at fixed rate—no contact contagion.

**Background**: Ads, official announcements.

**Principle**: r-shaped adoption curve.

**How to use**: Estimate reach rate; compare curve shape to diffusion/Bass.

**When to apply**: One-to-many dominant channel.

**When not**: Pure word-of-mouth/contact spread.

**Book anchor**: "Broadcast → r-shaped curve."

---

### Diffusion

**Definition**: Spread via **contact** between individuals.

**Background**: Word of mouth, behavioral contagion.

**Principle**: Slow → fast → saturate → S-curve.

**How to use**: Estimate contact & transmission rates; find inflection; combine with broadcast → Bass.

**When to apply**: Interpersonal/network contagion.

**When not**: Mass media only, no contact.

**Book anchor**: "Diffusion → S-shaped curve."

---

### Bass model

**Definition**: Broadcast + diffusion jointly; marketing standard.

**Background**: Products/ideas often dual-channel.

**Principle**: Parameters p (innovation), q (imitation); relative strength sets r vs S dominance.

**How to use**: Estimate p, q; fit adoption; allocate ad vs seed users.

**When to apply**: Both push and peer spread.

**When not**: Single channel → use broadcast or diffusion alone.

**Book anchor**: "r vs S depends on broadcast vs diffusion strength."

---

### SIR model

**Definition**: Susceptible → Infected → Recovered (may return to S); epidemic core.

**Background**: Disease, fading info, fashions.

**Principle**: R₀ = contact × spread / recovery; R₀>1 spreads, R₀<1 dies out; threshold.

**How to use**: Estimate rates; compute R₀ & herd immunity; interventions on contact/recovery/vaccination.

**When to apply**: Recoverable contagion; homogeneous or network-adjusted mix.

**When not**: Permanent adoption only; extreme heterogeneity needs network SIR.

**Book anchor**: "R₀>1 spreads; R₀<1 dies out."

---

## Uncertainty & path

### Entropy

**Definition**: Formal measure of uncertainty; low entropy = expected, high = surprise/information.

**Background**: Shannon; distinguish equilibrium/cycle/complexity/randomness.

**Principle**: Entropy ≠ variance; max-entropy under constraints; compare elections, prices, sequences.

**How to use**: Compare uncertainty across systems; subsequence entropy for dynamics; avoid ad hoc distributions.

**When to apply**: Uncertainty/information comparison; dynamic typing.

**When not**: Variance alone suffices.

**Book anchor**: "Information is the resolution of uncertainty." (Shannon)

---

### Random walk

**Definition**: Independent steps; Bernoulli urn with replacement; prices/performance with drift.

**Background**: Streaks vs skill; EMH baseline.

**Principle**: LLN → proportion convergence; long streaks exponentially rare; network structure affects return time.

**How to use**: Test if streak exceeds random expectation; skill-luck split; test price random-walkness.

**When to apply**: Independent increments; evaluate hot hands/win streaks.

**When not**: Mean reversion; structural alpha/trend.

**Book anchor**: "Elite shooters rarely hit nine threes in a row."

---

### Path dependence

**Definition**: Outcomes depend on history; dynamic urn (Polya) with positive feedback lock-in.

**Background**: QWERTY, institutions, precedents; vs critical points (sudden jumps).

**Principle**: Positive feedback → path-dependent equilibrium; negative feedback → path-dependent path but unique equilibrium possible.

**How to use**: Identify early accidents amplified; Polya thinking; ask reset cost.

**When to apply**: Behavior builds on others; positive feedback; switching costs.

**When not**: No feedback; costless reset; pure sudden criticality only.

**Book anchor**: "Path dependence is gradual; critical points are sudden."

---

### Local interaction

**Definition**: Cellular grid—local majority (match neighbor majority), Game of Life (complex rules).

**Background**: Coordination, segregation, emergence.

**Principle**: Local majority → equilibrium/patchy segregation; Life → any dynamic type; coordination paradox: local → global patchiness.

**How to use**: Define neighborhood & update rules; simulate long-run patches; Life for Explore not precise forecast.

**When to apply**: Spatial/neighbor imitation; cultural local alignment.

**When not**: Global mixing, one-shot full information.

**Book anchor**: "Local coordination → patchy, diverse global config."

---

## Equilibrium & dynamics

### Lyapunov functions

**Definition**: Real-valued L on configurations; strictly decreases each non-equilibrium step; bounded below → equilibrium.

**Background**: Convergence tests; contrast Life (no Lyapunov).

**Principle**: L exists → no cycles/chaos/complexity in that discrete system; may bound convergence time.

**How to use**: Construct potential (misaligned cells, total congestion); prove step decrease; if no L, don't assert convergence.

**When to apply**: "Will it settle?"—local majority, some markets, pure exchange.

**When not**: Life-like complexity; open-ended growth.

**Book anchor**: "Lyapunov function → must reach equilibrium."

---

### Markov models

**Definition**: States + transition probabilities; memoryless—next state depends only on current.

**Background**: Mood states, text transitions, PageRank, authorship.

**Principle**: Perron-Frobenius → unique stationary distribution; change **transitions** for long run, not just current state.

**How to use**: List states & matrix; find steady state; policy on structure not one-off state push.

**When to apply**: Markov approx OK; long-run shares matter.

**When not**: Long memory; non-stationary transitions; path history essential.

**Book anchor**: "Long-run change needs transition probabilities."

---

### Systems dynamics

**Definition**: Sources, sinks, stocks, flows, rates; positive feedback amplifies, negative stabilizes.

**Background**: Forrester; ecology, economy, supply chains.

**Principle**: Pure + → blow up/collapse; pure − → stability/cycles; both → complexity & counterintuitive indirect effects.

**How to use**: Draw stock-flow + feedback loops; mark delays/levers; don't fix stocks without fixing flows.

**When to apply**: Feedback loops, delays, accumulation; policy side effects.

**When not**: Static no-feedback; one-step decisions.

**Book anchor**: "Positive + negative feedback → complexity."

---

### Threshold models

**Definition**: Behavior flips when variable crosses threshold—riots, Schelling segregation, ABM granularity.

**Background**: Granovetter; tolerant agents can still segregate.

**Principle**: Threshold distribution → critical mass & cascades.

**How to use**: Estimate threshold distribution; find cascade tipping point; pick granularity fit for purpose.

**When to apply**: Discrete behavioral flips; participation, relocation, unrest.

**When not**: Smooth continuous response; no threshold.

**Book anchor**: "Threshold behavior can yield counterintuitive segregation."

---

## Choice, games & institutions

### Spatial competition

**Definition**: Options have **ideal points** in attribute space; closer = higher utility (spatial attributes).

**Background**: Product differentiation, candidate positioning.

**Principle**: Hotelling positioning; median voter (strong/weak); more attributes → sparser market, softer price competition.

**How to use**: Map spatial attributes; predict centripetal vs niche; adding dimensions as strategy.

**When to apply**: Heterogeneous ideal points; differentiation.

**When not**: Pure hedonic (more-is-better); over-simplified single ideology (Havel warning).

**Book anchor**: "Spatial attributes have no single optimal value."

---

### Hedonic competition

**Definition**: Valence attributes—more (or less) always better; hedonic regression for implicit prices.

**Background**: Square footage, battery life, durability.

**Principle**: Utility = weighted sum; regression coeffs = implicit marginal prices.

**How to use**: Price + attribute data → hedonic regression; check omitted attributes (pool value vs cost).

**When to apply**: Quantifiable attributes; market prices available.

**When not**: Pure taste/identity space; no transactions.

**Book anchor**: "For hedonic attributes, more is usually better."

---

### Game theory

**Definition**: Strategic interaction—payoffs depend on others; normal-form, sequential, continuous.

**Background**: Base for cooperation, signaling, mechanism design, collective action.

**Principle**: Dominance, Nash, subgame perfection; templates: zero-sum, entry, effort.

**How to use**: Players, strategies, payoffs; find equilibrium; repeated → cooperation possible.

**When to apply**: Strategic interdependence.

**When not**: No interaction; pure nature risk.

**Book anchor**: "From axioms through logic to predictions."

---

### Cooperation

**Definition**: Prisoner's dilemma structure—individual defection dominant, mutual cooperation better; repetition, reputation, networks sustain cooperation.

**Background**: Arms races, ad wars, public goods, evolution.

**Principle**: One-shot → defect; repeat + punishment → cooperate; network clustering spreads cooperation.

**How to use**: Check PD structure; time horizon, identification, punishment, network position; more links helps reputation vs low degree helps clustering—**conditional**.

**When to apply**: Free-rider vs collective gain; repeated/traceable.

**When not**: One-shot anonymous no sanction.

**Book anchor**: "Self-interest pursuit harms collective interest."

---

### Collective action & commons

**Definition**: Contribute c vs free-ride f; individual f better, all c best. Renewable resource/commons extension.

**Background**: Olson; fisheries, climate; no panacea.

**Principle**: Multi-player PD; growth-rate variance → collapse or abundance (non-canceling); context-specific institutions.

**How to use**: Map free-rider structure; combine repetition, exclusion, selective incentives; renewable—link harvest rules to growth variance.

**When to apply**: Public goods, commons, large-scale coordination.

**When not**: Private goods; fully priced markets.

**Book anchor**: "No panacea—no one-size-fits-all solution."

---

### Mechanism design

**Definition**: Design rules so self-interest yields desired outcomes—incentive compatible, IR, efficient, budget-balanced.

**Background**: FCC auctions, voting, public projects, second-price auctions.

**Principle**: Desiderata often incompatible; modeler as engineer; markets/democracy/hierarchy/collective action each fit some environments.

**How to use**: List goals; implement mechanism (VCG, pivot, second-price); accept tradeoffs.

**When to apply**: Rule design, auctions, voting, platform algorithms.

**When not**: No strategic behavior; pure description.

**Book anchor**: "Modeler becomes engineer of workable solutions."

---

### Signaling

**Definition**: Costly/verifiable signals separate types—education, brand, conspicuous consumption; pooling/separating/partial pooling.

**Background**: Veblen; Spence-style signaling games.

**Principle**: Signals must be costly or verifiable; separating = strong types only; pooling = all signal.

**How to use**: Hidden types & cost differential; analyze equilibrium type; policy: certification, audit.

**When to apply**: Information asymmetry; type affects action unobservable.

**When not**: Costless cheap talk; low-cost unverifiable signals.

**Book anchor**: "Signals must be costly or verifiable."

---

## Learning & search

### Learning models

**Definition**: Individual reinforcement (reward strengthens actions) & social learning (copy success/popularity); between rational and fixed rules.

**Background**: Gas-guzzler game—may converge risk-dominant not efficient.

**Principle**: Replicator dynamics; social learning amplifies via conformity + rewards, often faster than individual; equilibria may differ.

**How to use**: Environment: pick best alternative vs adapt in game; specify rule; predict convergence or cycles vs rational benchmark.

**When to apply**: Repeated decisions; observable others; behavior can change.

**When not**: One-shot high stakes full info → rational benchmark.

**Book anchor**: "Learning sits between rational choice and fixed rules."

---

### Multi-armed bandit

**Definition**: Arms with unknown reward distributions; **explore** vs **exploit** trade-off.

**Background**: Drug trials, ad placement, tech routes, careers.

**Principle**: Bernoulli bandit heuristics; general case Gittins index etc.

**How to use**: Define arms, priors, horizon; explore early, exploit late; compare to A/B/pilot design.

**When to apply**: Uncertain rewards; sequential/parallel trials OK.

**When not**: Known certain payoffs.

**Book anchor**: "Trade-off between exploration and exploitation."

---

### Rugged landscape

**Definition**: Fitness landscape over attribute combinations; NK model—high K → many local peaks, hard global optimum.

**Background**: Evolution, innovation search; Fuji landscape = single peak easy climb.

**Principle**: K=0 smooth; K=N−1 fully rugged; ~2^N/N local peaks; hill-climbing traps.

**How to use**: Assess multi-peak interaction; single peak → gradient search; rugged → diversity, jumps, parallel teams.

**When to apply**: Innovation, R&D, evolution, strategy with feature interactions.

**When not**: Known unimodal convex problem; additive no interaction.

**Book anchor**: "Too many local optima for hill-climbing alone."

---

## Problem → starter ensemble

| Prototype | Suggested trio |
|-----------|----------------|
| Why so top-heavy? | Power-law + preferential attachment + networks |
| Will it take off? | Bass/SIR + thresholds + networks |
| Policy works then fades? | Markov + systems dynamics + learning |
| Pilot then scale? | Bandit + diffusion + path dependence |
| Design the rules? | Mechanism design + games + signaling |
| Innovation stuck? | Rugged landscape + learning + networks |
