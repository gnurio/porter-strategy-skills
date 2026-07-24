---
name: design-competitive-move
description: >
  Design offensive or defensive competitive moves using Porter's framework. Use when planning competitive actions, responding to competitor moves, or managing industry discipline.
---

# Design Competitive Move

Design a competitive move that maximizes outcome through a combination of brute force (superior resources) and finesse (structuring the game so retaliation never begins).

## Input

- Competitor profile(s): goals, assumptions, current strategy, capabilities
- Firm's strategic position: strengths, weaknesses, resources, current commitments
- Proposed action: the move being considered (price change, market entry, product launch, etc.)

## Output

- Recommended move (cooperative or threatening) with rationale
- Expected competitor reactions: likelihood, speed, effectiveness, toughness
- Commitment requirements: what the firm must credibly stake
- Escalation risk: probability of destructive warfare

## Procedure

### Step 1: Classify the Move — Cooperative vs. Threatening

Evaluate whether the proposed move is **nonthreatening** or **threatening**.

**Cooperative (nonthreatening) moves** — three types:
1. Improves your position AND competitors' positions even if they do not match it
2. Improves your position AND competitors' positions only if a significant number match it
3. Improves your position because competitors will not match it (they don't perceive a need to)

**Threatening moves** — moves that improve your position at competitors' expense. Require predicting and managing retaliation. Evaluate:
1. How likely is retaliation?
2. How soon will retaliation come?
3. How effective will retaliation potentially be?
4. How tough will retaliation be (willingness to retaliate at own expense)?
5. Can retaliation be influenced?

**Always prefer cooperative moves when available.** They avoid the Prisoner's Dilemma: mutual cooperation yields reasonable profit for all, but self-interested moves invite destructive retaliation.

### Step 2: Exploit Mixed Motives

Search for moves where the competitor's retaliation would hurt their own broader business. A competitor caught in mixed motives faces internal conflict that creates a lag in retaliation — or prevents it entirely.

**Test each competitor against these questions:**
- Would retaliating cannibalize their most profitable product?
- Would it alienate their established distribution channels?
- Would it blur their premium brand image or strategic positioning?
- Would it force them to legitimize your concept?

**Examples from Porter:**
- Timex sold through drugstores, not jewelry stores. Swiss watchmakers couldn't retaliate without undermining jewelers and blurring their premium image. Retaliation never came.
- Bic's disposable razor put Gillette in a bind: reacting would cut into sales of their broad razor line — a dilemma Bic did not face.
- IBM was reluctant to enter minicomputers because the move would jeopardize mainframe sales.

### Step 3: Pick the Battleground

Select the market segment or strategic dimension where competitors are ill-prepared, least enthusiastic, or most uncomfortable competing. The ideal battleground is one where the legacy of their past strategy makes matching your move very costly, while posing less difficulty for you.

### Step 4: Design Commitment

Commitment communicates your resources and intentions unequivocally to remove uncertainty and force competitors to recalculate.

**Three types of commitment:**
1. **Stick with a move** — convince rivals you will not back down, so they resign themselves to the new position
2. **Retaliate** — convince rivals you will counter their moves with dogged, bitter force, deterring them from acting
3. **Take no action (create trust)** — convince rivals you will follow a price increase rather than undercut it, helping deescalate warfare

**Four pillars of credibility:**
1. **Visible assets** — excess cash, production capacity, fighting brands, large sales force, research facilities, small positions in competitor's other businesses usable for retaliation
2. **Clear intention** — consistent pattern of following through on past commitments; known defensive R&D programs already underway
3. **Irreversibility** — mechanisms that make backing down publicly embarrassing or financially ruinous: long-term contracts, plant purchases (not leases), public targets for market share, full integration rather than assembly
4. **Detection capability** — known systems for monitoring sales, talking to customers, interviewing distributors; competitors must believe cheating will be detected immediately

### Step 5: Establish Focal Points (Industry Discipline)

**Focal points** are prominent resting places where competitive expectations converge — standard price points, round-number market shares, geographic divisions, percentage markup rules.

**Three principles:**
1. Identify a desirable focal point as early as possible to minimize costly jockeying
2. Simplify industry variables (standard grades, standard products) so a focal point can emerge
3. Structure the game so the focal point best for your firm appears to emerge naturally (e.g., introduce terminology like "price per square foot" that favors your position)

**Discipline:** When a competitor steps out of line, deliver immediate retaliation aimed specifically at the aggressor. A fighting brand that copies the aggressor's product is more effective than a generalized response. Generalized retaliation (e.g., across-the-board price cuts) is more expensive, less effective, and risks triggering a chain reaction.

### Step 6: Design Defensive Moves

The most effective defense prevents the battle altogether through credible commitment to retaliate.

If a move has already occurred, use **"deny the base"**:
- Prevent the aggressor from meeting their growth, market share, or ROI targets within their time horizon
- If convinced targets will not be met for a long time, the competitor withdraws or deescalates
- **Tactics:** strong price competition, heavy R&D expenditure, attacking new products in test-market phase (cheaper than waiting for full launch), special deals to load customers with inventory (removing the market for the entrant)
- Essential prerequisite: a good hypothesis about the competitor's performance targets and time horizon

During synthesis, consult `reference.md` for Porter's heuristics on moves and commitment; before finalizing, check its failure modes.

## Output Template

```
## Move Classification
- Type: [Cooperative / Threatening]
- Subtype: [e.g., "improves both even without matching" or "mixed motives exploit"]

## Move Design
- Action: [specific move]
- Battleground: [segment/dimension chosen and why]
- Mixed motives check: [what retaliating costs the competitor]

## Expected Competitor Reactions
| Competitor | Likelihood | Speed | Effectiveness | Toughness |
|------------|-----------|-------|---------------|-----------|
| ...        | ...       | ...   | ...           | ...       |

## Commitment Plan
- Type: [stick with move / retaliate / create trust]
- Visible assets: [what you deploy]
- Irreversibility mechanism: [what makes backing down costly]
- Detection system: [how competitors know you'll detect cheating]

## Escalation Risk
- [Low/Medium/High] — [rationale]

## Defensive Provisions
- Deny-the-base plan: [if competitor counterattacks, how you prevent them from meeting targets]
- Focal point: [industry resting place you are promoting]
```

## Worked Example

**Situation:** A mid-market SaaS company (Firm A) wants to enter the enterprise segment currently dominated by Firm B, which has a premium brand, long-term contracts, and a direct sales force.

**Step 1 — Classification:** Threatening. Firm B's enterprise revenue is core to their goals; they will perceive an attack.

**Step 2 — Mixed motives:** Firm A prices 60% below Firm B with a self-serve onboarding model. If Firm B matches the price, they cannibalize their existing enterprise contracts and undermine the value proposition of their direct sales force. If they launch a self-serve tier, they blur their premium positioning. Firm B is caught in mixed motives.

**Step 3 — Battleground:** Mid-market companies expanding into enterprise needs — too small for Firm B's sales team to prioritize, but large enough to need enterprise features.

**Step 4 — Commitment:** Firm A publicly announces a $50M infrastructure investment and signs 3-year contracts with early enterprise customers (irreversibility). They publish a price guarantee (detection is easy — prices are public).

**Step 5 — Focal point:** Firm A introduces "cost per seat per month" as the industry metric, replacing Firm B's opaque annual contracts. This reframes the comparison in Firm A's favor.

**Step 6 — Defense:** If Firm B launches a downmarket product, Firm A denies the base by offering free migration tools and aggressive discounts to lock in the contested mid-market segment before Firm B can reach its year-one targets.

**Escalation risk:** Low-Medium. Mixed motives create a significant retaliation lag. Firm B's most rational response is to cede the low end and defend the premium enterprise core.
