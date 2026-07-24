---
name: diagnose-industry-type
description: >
  Classify an industry's evolutionary stage and structural type using Porter's criteria. Use when asked to diagnose industry maturity, identify if an industry is emerging/fragmented/declining, or understand industry evolution.
---

# Diagnose Industry Type

Classify an industry's evolutionary stage and structural type by matching observable market signals against Porter's diagnostic criteria, then route to the appropriate strategy skill.

## Input

- **Industry name** (required)
- **Observable market data**: growth rates, concentration ratios, buyer profiles, product innovation pace, competitive dynamics, capacity trends, profit trends

## Output

- Industry type classification (emerging | fragmented | transitioning to maturity | declining)
- Confidence level (high | medium | low)
- Key signals matched
- Recommended downstream skill for strategy formulation

## Procedure

1. **Gather signals.** List what is known about the industry across: growth trajectory, number/size of competitors, buyer sophistication, product standardization, capacity dynamics, profit trends, substitution threats, and regulatory shifts.
2. **Score against the 14 evolutionary processes** (below). Identify which processes are most active — this reveals the industry's evolutionary position.
3. **Run each classification checklist** (below). Count matching signals per type.
4. **If declining signals match**, apply the structural vs. cyclical decline test.
5. **Resolve conflicts.** An industry can be both fragmented AND emerging, or fragmented AND declining. If multiple types match, note the primary classification and secondary overlay.
6. **Assign confidence.** High = 5+ signals match one type clearly. Medium = 3-4 signals, or two types compete. Low = sparse data or ambiguous signals.
7. **Route** to the appropriate downstream skill.

## The 14 Evolutionary Processes (Diagnostic Signals)

These predictable dynamic processes occur in every industry. Assessing which are most active reveals evolutionary stage:

1. **Long-run changes in growth** — is the growth rate accelerating, plateauing, or declining?
2. **Changes in buyer segments served** — are new segments emerging or old ones shrinking?
3. **Buyers' learning** — are buyers becoming more experienced and sophisticated?
4. **Reduction of uncertainty** — is the technology/business model becoming proven?
5. **Diffusion of proprietary knowledge** — are trade secrets spreading? Are patents expiring?
6. **Accumulation of experience** — are cost curves flattening?
7. **Expansion (or contraction) in scale** — is the industry growing or shrinking in absolute terms?
8. **Changes in input and currency costs** — are cost structures shifting?
9. **Product innovation** — is the pace of new product introductions accelerating or slowing?
10. **Marketing innovation** — are new channels, positioning, or promotional methods emerging?
11. **Process innovation** — are manufacturing or delivery methods being reinvented?
12. **Structural change in adjacent industries** — are suppliers, buyers, or complementors changing?
13. **Government policy change** — are regulations tightening, loosening, or shifting?
14. **Entries and exits** — are new firms flooding in, or are incumbents leaving?

## Classification Checklists

### Emerging Industry

- [ ] Created by technological innovation, shifts in relative cost relationships, or emergence of new consumer needs
- [ ] "No rules of the game" — competitive rules are still being established
- [ ] High uncertainty about technology, strategy, and market size
- [ ] Many new entrants experimenting with different approaches
- [ ] First-time buyers dominate; no repeat-purchase pattern yet
- [ ] Proprietary knowledge is closely held; little diffusion

### Fragmented Industry

- [ ] No firm has a significant market share or can strongly influence industry outcomes
- [ ] Large number of small- and medium-sized companies, many privately held
- [ ] Absence of market leaders with power to shape industry events
- [ ] Low barriers to entry
- [ ] Diseconomies of scale or other structural reasons preventing consolidation

### Transitioning to Maturity

- [ ] Slowing growth sparks increased competition for market share
- [ ] Sales increasingly shift to experienced, repeat buyers
- [ ] Competition places greater emphasis on cost and service
- [ ] "Topping-out" problem: capacity additions must slow or overcapacity results
- [ ] Manufacturing, marketing, distribution, and research methods undergoing change
- [ ] New products and applications become harder to discover
- [ ] International competition increases
- [ ] Industry profits fall during the transition period
- [ ] Dealer margins squeezed, but dealer power increases as manufacturers compete for distribution

### Declining Industry

- [ ] Absolute decline in unit sales over a sustained period
- [ ] Decline driven by technological substitution, demographics, or shifts in buyer needs/tastes
- [ ] Capacity exceeds demand; exit barriers trap competitors
- [ ] Surviving firms compete for shrinking pie

## Structural vs. Cyclical Decline Test

Porter is explicit: true structural decline **cannot be ascribed to the business cycle or short-term discontinuities** (strikes, material shortages). Apply this test:

| Factor | Structural Decline | Cyclical Downturn |
|---|---|---|
| Duration | Sustained, multi-year | Tied to economic cycle |
| Cause | Technological substitution, demographic shifts, permanent changes in buyer needs | Recession, temporary supply disruption |
| Reversibility | Irreversible without fundamental reinvention | Self-correcting as cycle turns |
| Substitutes | Growing substitute eroding demand permanently | No new substitute; demand returns |

If structural: route to end-game strategy. If cyclical: do not classify as declining — reassess at next cycle.

## Routing Logic

| Classification | Downstream Skill |
|---|---|
| Emerging | `strategize-emerging-industry` |
| Fragmented | `strategize-fragmented-industry` |
| Transitioning to maturity | `select-generic-strategy` -- no dedicated maturity skill exists; Porter's maturity advice (compete on cost/service, rationalize product mix) is closest to generic-strategy selection |
| Declining | `strategize-declining-industry` |
| Ambiguous / multi-type | Re-gather data or present both classifications with caveats |

During synthesis, consult `reference.md` for Porter's heuristics on industry evolution; before finalizing, check its failure modes.

## Output Template

```
## Industry Diagnosis: [Industry Name]

**Classification:** [Emerging | Fragmented | Transitioning to Maturity | Declining]
**Confidence:** [High | Medium | Low]

### Signals Matched
- [Signal 1]
- [Signal 2]
- ...

### Active Evolutionary Processes
- [Process name]: [observation]
- ...

### Structural vs. Cyclical Assessment (if declining)
[Assessment]

### Recommended Next Step
→ Route to: `[downstream skill name]`
→ Rationale: [why this classification leads to this skill]
```

## Worked Example

**Industry:** U.S. traditional print newspaper publishing (circa 2015)

**Signals matched (Declining):**
- Absolute decline in unit sales (circulation) sustained over 10+ years
- Technological substitution: digital news consumption replacing print
- Demographic shift: younger cohorts never adopted print habit
- Shift in buyer needs: advertisers migrating spend to digital platforms
- Capacity exceeds demand: printing presses underutilized, bureaus closing

**Active evolutionary processes:**
- Long-run changes in growth: negative, accelerating decline
- Diffusion of proprietary knowledge: news content freely available online
- Structural change in adjacent industries: advertising industry shifted to digital
- Entries and exits: multiple exits (closures, mergers); few entries

**Structural vs. cyclical test:** Decline persists through both recession and recovery periods. Driven by permanent technological substitution (digital) and demographic shifts, not economic cycles. Verdict: **structural decline.**

**Classification:** Declining (structural)
**Confidence:** High (6+ signals, clear structural cause)
**Route to:** `strategize-declining-industry`
