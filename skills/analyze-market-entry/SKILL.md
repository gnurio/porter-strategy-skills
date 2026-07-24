---
name: analyze-market-entry
description: >
  Evaluate market entry opportunities using Porter's entry analysis framework. Use when asked to assess whether to enter a new market, how to enter, or what entry barriers exist.
---

# Analyze Market Entry

Evaluate whether and how to enter a new business by balancing structural barriers, retaliation costs, and the entrant's distinctive capabilities.

## Input

- **Target industry**: the business or market segment under consideration
- **Entrant's current capabilities**: existing businesses, assets, distribution, technology, brand, and capital

## Output

- Go/no-go recommendation with confidence level
- Recommended entry mechanism (from generic entry concepts)
- Barrier-by-barrier cost analysis
- Retaliation scenario modeling
- If acquisition is relevant: market-for-companies assessment

## Procedure

### Step 1: Estimate total entry cost

Balance four factors (Porter's entry equation):

1. **Basic investment costs** -- facilities, inventory, sales force, working capital
2. **Costs to overcome structural entry barriers** -- brand franchise, tied-up distribution, proprietary technology, access to raw materials, economies of scale
3. **Expected cost of incumbent retaliation** -- magnitude of adverse effects multiplied by probability of occurrence
4. **Expected cash flows from being in the industry** -- discounted future returns

Do NOT stop at visible capital costs. Calculate the up-front investments and start-up losses required to replicate intangible advantages (brand identification, channel access, proprietary technology). Also estimate whether entry will artificially inflate prices of scarce supplies, equipment, or labor.

### Step 2: Model incumbent retaliation

Retaliation is an explicit cost: (financial impact of retaliation) x (probability it occurs).

Forecast the **extent** and **duration** of the reaction. Adjust pro forma prices and costs accordingly.

Retaliation is most likely when:
- Industry growth is slow (entry takes absolute sales from incumbents)
- Products are commodities (no brand loyalty or segments to insulate)
- Fixed costs are high (added capacity destroys utilization)
- Incumbents attach high strategic importance to the business (cash flow dependence, flagship status, interrelationships)
- Incumbent management has emotional attachment (long-established, single-business companies treat entry as an affront)

### Step 3: Select entry mechanism

Choose from Porter's **generic entry concepts** -- ways to overcome barriers more cheaply than other firms:

| Concept | How it works |
|---|---|
| **Reduce product costs** | New process technology, larger plant with greater scale economies, more modern facilities, or shared activities with existing businesses |
| **Buy in with low price** | Sacrifice short-term returns through aggressive pricing to force competitors to yield share; depends on competitors' unwillingness or inability to retaliate |
| **Offer a superior product** | Product or service innovation that overcomes existing differentiation barriers |
| **Discover a new niche** | Find an unrecognized market segment with distinctive requirements, bypassing differentiation and distribution barriers |
| **Introduce a marketing innovation** | New marketing methods that circumvent distributor power or build brand identification |
| **Use piggybacked distribution** | Build entry on distribution relationships already established by the entrant's other businesses |
| **Sequenced entry** | Enter a low-barrier strategic group first (e.g., private label manufacturing), accumulate capital, experience, and brand recognition, then shift into the ultimate target group |

### Step 4: Evaluate sequenced entry option

Sequenced entry lowers total cost and risk by:
- Accumulating knowledge and brand identification in an initial group, then using it at no cost for mobility into the target group
- Developing managerial talent in a measured way
- Tempering incumbent reaction (less threatening initial move)
- Segmenting risk -- if the initial entry fails, the firm is spared the cost of going further
- Allowing capital accumulation for subsequent shifts in position
- Permitting first-step entry into a group requiring relatively reversible investments (e.g., saleable plant capacity) before committing to irreversible ones (advertising, R&D)

### Step 5: Assess entry via acquisition

Acquisition does not add a new firm to the industry. Price is set in the **market for companies** -- an efficient marketplace of buyers, sellers, and brokers. Efficiency tends to bid up prices and eliminate above-average returns.

An acquisition yields above-average returns only when at least two of three conditions hold:

1. **Low floor price** -- the seller is compelled to sell (estate problems, capital needs, no management successors, low confidence in own prospects)
2. **Imperfect market for companies** -- few bidders, bad economy, sick target company, buyer has superior information
3. **Unique ability to operate the acquired business** -- buyer has distinctive assets or skills that improve the target's strategic position beyond what other bidders can achieve

Compare: internal development requires a distinctive ability to overcome entry barriers cheaply; acquisition requires a distinctive ability to outbid others and still earn above-average profits.

### Step 6: Synthesize go/no-go recommendation

Weigh total entry cost (barriers + retaliation) against expected industry cash flows. Recommend entry only when:
- The entrant has a distinctive advantage that lowers barrier costs below what rivals face
- Retaliation can be absorbed or mitigated by the chosen entry mechanism
- Expected returns exceed the full cost of entry including intangible barrier costs

During synthesis, consult `reference.md` for Porter's heuristics on entry economics; before finalizing, check its failure modes.

## Output Template

```
## Entry Analysis: [Target Industry]

### 1. Structural Barrier Assessment
| Barrier | Severity | Estimated Cost to Overcome |
|---------|----------|---------------------------|
| [barrier] | High/Med/Low | [cost or investment required] |

### 2. Retaliation Forecast
- Probability of retaliation: [High/Med/Low]
- Triggers: [slow growth / commodity product / high fixed costs / strategic importance]
- Expected form: [price cuts / marketing escalation / capacity expansion]
- Estimated duration: [months/years]
- Cost adjustment to pro forma: [amount or percentage]

### 3. Recommended Entry Mechanism
- Primary: [generic concept from Porter]
- Rationale: [why this concept fits the entrant's capabilities]
- Sequenced entry option: [if applicable, describe stepping-stone group]

### 4. Acquisition Alternative
- Floor price assessment: [high/low, with reasons]
- Market efficiency: [number of bidders, economy conditions]
- Unique operating ability: [what the entrant can do that others cannot]
- Verdict: [acquire vs. build internally]

### 5. Go/No-Go Recommendation
- Recommendation: [GO / NO-GO / CONDITIONAL]
- Confidence: [High/Med/Low]
- Key assumption: [the single factor most likely to invalidate this analysis]
```

## Worked Example

**Scenario**: A consumer electronics company with strong retail distribution considers entering the premium home appliance market.

**Step 1 -- Barriers**: High brand identification (established incumbents like Miele, Sub-Zero). Distribution partially accessible via existing retail relationships. Moderate economies of scale. Proprietary technology in some segments. Estimated barrier cost: $200M over 3 years in brand-building and product development.

**Step 2 -- Retaliation**: Industry growth is moderate (5%). Products are differentiated, not commodities. Incumbents have high strategic attachment. Retaliation probability: Medium. Expected form: increased marketing spend, loyalty programs. Estimated pro forma adjustment: -8% on revenue projections for years 1-3.

**Step 3 -- Mechanism**: **Use piggybacked distribution** (leverage existing retail relationships) combined with **offer a superior product** (smart-home integration that incumbents lack).

**Step 4 -- Sequenced entry**: Enter via small appliances first (lower barriers, reversible investment), build brand recognition, then expand into large premium appliances. This segments risk and accumulates industry knowledge.

**Step 5 -- Acquisition**: One mid-tier appliance brand available. Floor price moderate (seller is optimistic about prospects). Few competing bidders (niche market). Entrant has distinctive ability to add smart-home technology and distribution. Verdict: acquisition viable but not clearly superior to sequenced internal entry.

**Step 6 -- Recommendation**: CONDITIONAL GO via sequenced entry. Enter small appliances leveraging existing distribution, prove the brand, then expand. Key assumption: retail partners will allocate shelf space to a new appliance brand from an electronics company.
