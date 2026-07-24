---
name: orchestrate-porter-strategy
description: >
  Route competitive strategy analysis to the right Porter skill. Use when asked for broad competitive analysis, industry assessment, strategy formulation, or any Porter-related question.
---

# Orchestrate Porter Strategy

Route the user's request to the correct Porter skill(s) and chain outputs into a coherent analysis.

## Skill Registry

| Skill | Accepts | Produces | Use When |
|-------|---------|----------|----------|
| analyze-five-forces | Industry name | Force-by-force assessment, governing forces, profit potential | "analyze industry", "competitive dynamics", "industry attractiveness", "profit potential" |
| profile-competitor | Competitor name + industry | 4-component profile, response predictions, blind spots | "analyze competitor", "predict moves", "competitive threat" |
| map-strategic-groups | Industry + competitor list | Group map, mobility barriers, positioning gaps | "segment competitors", "strategic groups", "positioning", "mobility barriers" |
| diagnose-industry-type | Industry + market data | Type classification + routed recommendation | "industry maturity", "emerging/fragmented/declining", "industry evolution" |
| select-generic-strategy | Five forces + group position | Strategy recommendation + requirements + stuck-in-the-middle verdict | "cost leadership vs differentiation", "generic strategy", "stuck in the middle" |
| read-market-signals | Competitor action/announcement | Signal classification, bluff vs. commitment, recommended response | "decode announcement", "competitor signal", "cross-parry", "fighting brand" |
| analyze-market-entry | Target industry + capabilities | Go/no-go + entry mechanism + retaliation scenarios | "enter new market", "entry barriers", "acquisition vs organic" |
| strategize-fragmented-industry | Industry diagnosis + firm position | Consolidate vs. cope + specific strategy | "fragmented industry", "many small competitors", "consolidation" |
| strategize-emerging-industry | Industry diagnosis + capabilities | Strategic posture + scenarios + monitoring agenda | "emerging industry", "new market", "pioneer vs follower" |
| strategize-declining-industry | Industry diagnosis + firm position | End-game strategy recommendation | "declining industry", "shrinking demand", "exit strategy" |
| design-competitive-move | Competitor profile + position + action | Move design + reactions + commitment + escalation risk | "competitive move", "respond to competitor", "offensive/defensive strategy" |
| audit-strategy-consistency | Current strategy (goals + policies) | Pass/fail per test + overall verdict | "strategy consistent?", "strategy audit", "strategic drift" |

## Routing Rules

### Step 1: Detect Entry Point

Match the user's request to one or more entry-point skills:

- **Industry-level question** → `analyze-five-forces` (then optionally `diagnose-industry-type`)
- **Competitor question** → `profile-competitor` (then optionally `read-market-signals`)
- **Positioning question** → `map-strategic-groups`
- **"What strategy should we pursue?"** → `select-generic-strategy` (needs five forces + groups first)
- **Market entry question** → `analyze-market-entry`
- **Competitor action/signal** → `read-market-signals`
- **"How should we respond/attack?"** → `design-competitive-move` (needs competitor profile first)
- **"Is our strategy coherent?"** → `audit-strategy-consistency`
- **Industry type explicitly stated** → route directly to `strategize-{fragmented|emerging|declining}-industry`

If ambiguous, ask: "Are you trying to understand the industry, analyze a competitor, choose a strategy, or plan a move?"

### Step 2: Chain Outputs

After each skill completes, check if its output feeds a downstream skill:

```
analyze-five-forces ──→ select-generic-strategy
                    ──→ analyze-market-entry
map-strategic-groups ──→ select-generic-strategy
diagnose-industry-type ──→ strategize-{fragmented|emerging|declining}-industry
profile-competitor ──→ read-market-signals
                   ──→ design-competitive-move
select-generic-strategy ──→ design-competitive-move
                        ──→ audit-strategy-consistency
```

Only chain if the user's question warrants it. Don't run the full DAG for a simple question.

### Step 3: Skip Logic

- Skip a skill if its output is already supplied by the user
- Skip industry-type strategies if `diagnose-industry-type` classifies as "mature/stable" (no specialized strategy needed)
- Skip `design-competitive-move` unless the user has a specific action in mind

## Workflow Shortcuts

For common multi-skill analyses, use these pre-built chains:

### Quick Industry Check
`analyze-five-forces` → `diagnose-industry-type` → (route to industry-type skill if applicable)
**Trigger:** "analyze this industry", "how attractive is this market?"

### Competitor Deep Dive
`profile-competitor` → `read-market-signals` (if recent actions exist)
**Trigger:** "analyze [competitor]", "what will [competitor] do?"

### Should We Enter?
`analyze-five-forces` → `analyze-market-entry`
**Trigger:** "should we enter [market]?", "entry barriers"

### What Move?
`profile-competitor` → `select-generic-strategy` → `design-competitive-move`
**Trigger:** "how should we compete?", "what move should we make?"

### Full Strategic Audit
`analyze-five-forces` → `map-strategic-groups` → `select-generic-strategy` → `audit-strategy-consistency`
**Trigger:** "full competitive analysis", "comprehensive strategy review"

## Environment Assumptions

All skills assume: the user can provide an industry name and basic context; analysis is for a specific firm competing in the industry, not academic; data may be incomplete, so skills should note gaps rather than hallucinate.

## Context Accumulation

As skills execute, accumulate their outputs in a running context object. Pass relevant prior outputs as input to downstream skills. Present the accumulated analysis to the user at the end.

## Edge Cases

- **Multiple industries:** Run the chain separately for each, then compare
- **Diversified firm:** Run per-business-unit, noting corporate portfolio effects (from `profile-competitor` parent company analysis)
- **No clear competitor:** Start with `analyze-five-forces` and `map-strategic-groups` before attempting competitor analysis
- **User wants everything:** Use the Full Strategic Audit workflow, but warn it requires substantial input data
