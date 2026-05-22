---
name: select-generic-strategy
description: >
  Select the right generic competitive strategy using Porter's framework. Use when asked to choose between cost leadership, differentiation, or focus, or to diagnose being stuck in the middle.
---

# Select Generic Strategy

Determine which of Porter's three generic strategies best fits a firm's competitive situation, verify the firm can meet its requirements, and diagnose whether it is stuck in the middle.

## Input

- Five forces assessment (from `analyze-five-forces` skill)
- Strategic group position (from `map-strategic-groups` skill)
- Firm's current resources, capabilities, and organizational profile

## Output

- Recommended generic strategy (cost leadership | differentiation | focus)
- Requirements checklist: skills/resources, organizational arrangements, control/incentive systems
- Strategy-specific risks
- Stuck-in-the-middle verdict (yes/no + evidence)
- Feasibility of dual-strategy pursuit

## Procedure

1. Summarize the firm's five forces profile and strategic group position.
2. Evaluate each generic strategy against the firm's situation using the requirements tables below.
3. Identify which strategy the firm can most credibly commit to with "total commitment and supporting organizational arrangements."
4. Run the stuck-in-the-middle diagnostic.
5. Assess risks of the recommended strategy.
6. Deliver recommendation with requirements gap analysis.

## Strategy Profiles

### 1. Overall Cost Leadership

| Category | Requirements |
|---|---|
| **Skills & Resources** | Sustained capital investment and access to capital; process engineering skills; intense supervision of labor; products designed for ease of manufacture; low-cost distribution system |
| **Org Arrangements** | Structured organization and responsibilities; tight cost control |
| **Control / Incentives** | Frequent, detailed control reports; incentives based on meeting strict quantitative targets |

**Risks:**
- Technological change nullifies past investments or learning
- Low-cost learning by newcomers or followers through imitation or investment in state-of-the-art facilities
- Inability to see required product or marketing changes due to attention placed on cost
- Inflation in costs narrows the price differential needed to offset competitors' brand images or differentiation

### 2. Differentiation

| Category | Requirements |
|---|---|
| **Skills & Resources** | Strong marketing abilities; product engineering; creative flair; strong capability in basic research; corporate reputation for quality or technological leadership; long tradition in the industry or unique combination of skills drawn from other businesses; strong cooperation from channels |
| **Org Arrangements** | Strong coordination among functions in R&D, product development, and marketing; amenities to attract highly skilled labor, scientists, or creative people |
| **Control / Incentives** | Subjective measurement and incentives instead of quantitative measures |

**Risks:**
- Cost differential between low-cost competitors and the differentiated firm becomes too great for differentiation to hold brand loyalty -- buyers sacrifice features for large cost savings
- Buyers' need for the differentiating factor falls as they become more sophisticated
- Imitation narrows perceived differentiation, a common occurrence as industries mature

### 3. Focus

| Category | Requirements |
|---|---|
| **Skills & Resources** | Combination of cost leadership or differentiation policies directed at the particular strategic target |
| **Org Arrangements** | Combination of above, directed at the particular strategic target |
| **Control / Incentives** | Combination of above, directed at the particular strategic target |

**Risks:**
- Cost differential between broad-range competitors and the focused firm widens, eliminating cost advantages of serving a narrow target or offsetting the differentiation achieved by focus
- Differences in desired products or services between the strategic target and the market as a whole narrow
- Competitors find sub-markets within the strategic target and "outfocus" the focuser

## Stuck-in-the-Middle Diagnostic

A firm is stuck in the middle when it "lacks the market share, capital investment, and resolve to play the low-cost game, the industrywide differentiation necessary to obviate the need for a low-cost position, or the focus to create differentiation or a low-cost position in a more limited sphere."

**Checklist -- flag YES/NO for each:**

1. Low profitability relative to industry peers
2. Losing high-volume customers to lower-cost competitors
3. Losing high-margin customers to focused or differentiated firms
4. Blurred corporate culture -- no clear strategic identity
5. Conflicting organizational arrangements and motivation systems
6. No clear commitment to any one generic strategy

**Verdict:** 3+ flags = likely stuck in the middle. The firm must make a "fundamental strategic decision": either invest aggressively to achieve cost leadership/parity, orient to a particular target (focus), or achieve some uniqueness (differentiation). The latter two may require shrinking market share or absolute sales.

## Can a Firm Pursue More Than One Generic Strategy?

Porter's position: "Sometimes the firm can successfully pursue more than one approach as its primary target, though this is rarely possible." Being the lowest-cost producer and being truly differentiated are "rarely compatible." The core problem: each strategy requires different resources, strengths, organizational arrangements, and managerial style, which are "diluted if there is more than one primary target."

**Porter's examples of apparent dual success:**
- **GE (electric motors):** Achieved large market share and strong cost position while maintaining a strong technological reputation. Industry economics permitted it.
- **Microsoft:** Got "so far ahead that they seem to avoid the need for strategic choices" -- but Porter warns this "becomes their ultimate vulnerability."

**Conditions that must hold:**
1. The industry's economics must allow low overall cost to not be fundamentally incompatible with the added expenses of differentiation.
2. Firms should not forgo improvements in one dimension that "involve no sacrifice in the other" -- but this is operational effectiveness, not strategic position.
3. Porter distinguishes operational effectiveness (no tradeoff, all firms should pursue) from strategic position (requires choice). Confusing the two is a common error.

**Default recommendation:** Pick one strategy and commit totally. Pursuing two as primary targets usually produces stuck-in-the-middle outcomes.

## Heuristics

- Cost leadership demands a firm be THE cost leader, not one of several. Failing to achieve this leaves the firm "in an extremely poor strategic situation."
- Differentiation does not mean ignoring costs -- but cost is not the primary strategic target.
- Focus works by serving a narrow target "more effectively or efficiently" than broad competitors. It achieves either low cost or differentiation (or both) within its segment.
- Each strategy requires "total commitment." Half-measures produce stuck-in-the-middle outcomes.
- Different strategies "require different styles of leadership and can translate into very different corporate cultures." Different sorts of people will be attracted.

## Failure Modes

1. **Attempting cost leadership without scale or capital access** -- leads to cost disadvantage, not advantage
2. **Differentiating on attributes buyers do not value** -- pays the cost of differentiation without the premium
3. **Focusing on a segment too similar to the broader market** -- broad competitors serve it equally well
4. **Hedging across strategies** -- "conflicting organizational arrangements and motivation systems" guarantee mediocrity
5. **Ignoring risks** -- e.g., a cost leader blind to product/marketing shifts (Ford 1920s)
6. **Confusing operational effectiveness with strategy** -- efficiency improvements are not a generic strategy

## Output Template

```
## Generic Strategy Recommendation

**Firm:** [name]
**Recommended Strategy:** [Cost Leadership | Differentiation | Focus]
**Confidence:** [High | Medium | Low]

### Requirements Fit
| Requirement | Firm Status | Gap? |
|---|---|---|
| [from table above] | [met/partial/unmet] | [description] |

### Key Risks
- [top 2-3 risks from the relevant strategy]

### Stuck-in-the-Middle Verdict
- [ ] Low profitability
- [ ] Losing volume customers to cost leaders
- [ ] Losing margin customers to differentiators/focusers
- [ ] Blurred corporate culture
- [ ] Conflicting org arrangements / incentives
- [ ] No clear strategic commitment
**Verdict:** [Stuck / Not stuck]

### Dual-Strategy Assessment
[Can the firm credibly pursue a second strategy? Why / why not?]

### Action Items
1. [Highest-priority gap to close]
2. [Second priority]
3. [Third priority]
```

## Worked Example

**Firm:** Regional grocery chain, mid-market, 40 stores

**Five Forces Summary:** High buyer power (price-sensitive consumers), moderate supplier power, high rivalry (national chains + discounters), low threat of new entry, moderate substitutes (meal kits, restaurants).

**Strategic Group:** Mid-tier -- neither cheapest nor most premium. Competes with both Walmart (cost leader) and Whole Foods (differentiator).

**Requirements Fit (Cost Leadership):** Cannot match Walmart's scale, capital access, or distribution system. Lacks process engineering depth. Verdict: unfit.

**Requirements Fit (Differentiation):** No corporate reputation for quality or technological leadership. Weak marketing capabilities. Verdict: unfit at industry-wide level.

**Requirements Fit (Focus):** Can serve local/regional customers with curated local products, superior fresh departments, and community relationships. Has strong channel cooperation with local suppliers. Org can be restructured around the target segment.

**Recommendation:** Focus strategy -- serve the "local/premium fresh" segment more effectively than broad-range competitors. Requires: restructuring incentives around customer satisfaction (subjective measures), investing in local supplier relationships, and accepting loss of price-sensitive volume customers.

**Stuck-in-the-Middle Verdict:** Currently YES (4/6 flags). The focus pivot resolves this by committing fully to a narrow target.
