---
name: strategize-declining-industry
description: >
  Choose an end-game strategy for declining industries using Porter's framework. Use when demand is structurally shrinking, industry is contracting, or firms are exiting.
---

# Strategize Declining Industry

Choose an end-game strategy (Leadership, Niche, Harvest, or Divest) by matching the hospitability of the declining industry against the firm's relative competitive strengths.

## Input

- Industry diagnosis from `diagnose-industry-type` confirming structural decline
- Firm's competitive position: assets, strengths, market share, exit barriers
- Cause of decline (substitution, demographic shift, regulatory change, etc.)

## Output

- Decline hospitability rating (hospitable / inhospitable) with factor-by-factor assessment
- Exit barrier profile for each significant competitor
- Recommended end-game strategy with rationale
- Tactical steps for executing the chosen strategy

## Procedure

### Step 1 — Assess Decline Hospitability

Rate each factor as hospitable or inhospitable:

| Factor | Hospitable | Inhospitable |
|--------|-----------|--------------|
| **Uncertainty of demand** | Firms are certain decline will continue; inefficient firms plan orderly withdrawal | Firms perceive hopes of revitalization; competitors hang on, sparking warfare |
| **Nature of remaining demand** | Remaining pockets are price-insensitive (e.g., replacement parts), immune to substitution, buyers lack bargaining power | Remaining demand is commodity-like, price-sensitive, threatened by further substitutes |
| **Exit barriers** | Low across the industry; capacity leaves the market in orderly fashion | High; firms are trapped, capacity stays, competition intensifies |
| **Volatility of rivalry** | Differentiated products, low fixed costs, few competitors | Commodity products, high fixed costs, many equally balanced firms, high strategic stakes |

Overall verdict: hospitable if most factors align favorably. Inhospitable if firms are trapped and warfare is likely.

### Step 2 — Analyze Exit Barriers for Each Competitor

For every significant competitor, assess:

1. **Specialized assets** — Is equipment highly specialized with low liquidation value, or can it be sold (including to overseas markets)?
2. **Fixed costs of exit** — Labor settlements, contract cancellation penalties, spare parts obligations?
3. **Strategic interrelationships** — Is the business central to corporate identity? Does it share facilities or distribution channels with other divisions?
4. **Vertical integration** — Will closing this unit force closure of upstream or downstream facilities?
5. **Managerial/emotional barriers** — Intense pride or loyalty preventing rational exit?
6. **Government/social restrictions** — Will government or community pressure block exit to prevent job losses?

Predict: who will exit quickly, who will remain, and who will fight bitterly.

### Step 3 — Assess the Firm's Own Position

- What are the firm's exit barriers (same six factors)?
- What are the firm's relative strengths for the remaining pockets of demand? (These may differ from strengths that mattered earlier in the industry's life.)
- Does the firm have credibility to prompt competitors to exit?
- What are the firm's overarching strategic needs (e.g., need for cash flow) that may skew the decision?

### Step 4 — Select End-Game Strategy Using the 2x2 Matrix

|  | **Has Strengths** for remaining demand | **Lacks Strengths** for remaining demand |
|--|---------------------------------------|------------------------------------------|
| **Favorable industry structure** | **Leadership** or **Niche** | **Harvest** or **Divest Quickly** |
| **Unfavorable industry structure** | **Niche** (shrink into protected segment) or **Harvest** | **Divest Quickly** |

#### The Four Strategies

1. **Leadership** — Become the only (or one of few) remaining firms. Prompt competitors to exit through aggressive pricing, acquisitions, or capacity signaling. Once dominant, switch to holding position or controlled harvest. *Requires:* favorable industry structure AND competitive strengths AND credibility to prompt exits.

2. **Niche** — Create or defend a strong position in a specific, stable segment. Works in favorable industries (choose the best segment) and can work in unfavorable industries if the firm shrinks into a highly protected pocket. *Requires:* strengths in a particular segment where demand is durable.

3. **Harvest** — Controlled disinvestment to optimize cash flow. Ultimately sell or liquidate. Two categories of tactics:
   - *Visible actions:* Raise prices, reduce models, shrink channels, erode service (delivery time, repair speed, sales assistance). Only viable if the firm has genuine past strengths (brand loyalty, goodwill).
   - *Invisible actions:* Defer facility maintenance, drop marginal accounts. Firms without strong market positions must confine themselves to invisible actions only.
   *Requires:* genuine past strengths to live on, and an environment that does not degenerate into bitter warfare. *Warning:* administratively very difficult — devastates employee morale and retention, destroys supplier/customer confidence, and offers terrible motivation for executives managing the "dog."

4. **Divest Quickly** — Liquidate the investment as early as possible in the decline phase. Divesting early maximizes asset resale value before the decline is universally recognized. *Best when:* firm lacks strengths AND industry structure is unfavorable. Consider divesting even before decline is obvious if forecast is confident.

### Step 5 — Overlay Strategic Needs

A firm's corporate-level needs (cash flow requirements, portfolio balance, identity considerations) may override the matrix. For example, cash flow urgency may push toward Harvest or Divest even when the matrix suggests Leadership.

During synthesis, consult `reference.md` for Porter's heuristics on decline; before finalizing, check its failure modes.

## Output Template

```
## End-Game Strategy: [Industry Name]

### Decline Hospitability Assessment
- Uncertainty of demand: [hospitable/inhospitable] — [rationale]
- Nature of remaining demand: [hospitable/inhospitable] — [rationale]
- Exit barriers (industry-wide): [hospitable/inhospitable] — [rationale]
- Volatility of rivalry: [hospitable/inhospitable] — [rationale]
- Overall: [HOSPITABLE / INHOSPITABLE]

### Competitor Exit Barrier Profiles
| Competitor | Specialized Assets | Fixed Costs | Strategic Ties | Vertical Integration | Emotional | Gov't | Likely Action |
|------------|-------------------|-------------|----------------|---------------------|-----------|-------|---------------|
| [Name]     | [H/M/L]          | [H/M/L]    | [H/M/L]       | [H/M/L]            | [H/M/L]  | [H/M/L] | [Exit/Stay/Fight] |

### Firm's Position
- Exit barriers: [summary]
- Strengths for remaining demand: [summary]
- Credibility to prompt exits: [Y/N — why]
- Strategic needs override: [if any]

### Recommended Strategy: [LEADERSHIP / NICHE / HARVEST / DIVEST QUICKLY]
Rationale: [2-3 sentences linking hospitability + firm position to strategy choice]

### Tactical Steps
1. [Action]
2. [Action]
3. [Action]
```

## Worked Example: Vacuum Tube Industry (1960s-1970s)

**Hospitability:** Inhospitable. Transistors were a clear substitute, but remaining demand (replacement tubes for existing equipment, color TV sets in early years) created uncertainty about the pace of decline. High fixed costs of manufacturing. Assets highly specialized.

**Competitor exit barriers:** Most firms had specialized plant with low liquidation value. Raytheon had low emotional barriers and sold assets early (early 1960s) when color TV demand was strong, recovering high value. Firms that waited until the 1970s found few buyers and weak bargaining position.

**Firm position (Raytheon):** Had relative strength in early period but recognized decline trajectory. No strategic interrelationships tying them to the business. Low emotional barriers.

**Strategy chosen: Divest Quickly.** Raytheon sold its vacuum tube assets in the early 1960s, recovering substantial liquidation value. Firms that stayed faced an increasingly inhospitable environment as overseas producers entered with lower cost structures and remaining demand eroded further.

**Key lesson:** Divesting early — before decline was universally recognized — maximized asset value. Waiting destroyed bargaining position.
