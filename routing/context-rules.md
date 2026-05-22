# Routing Context Rules

## Activation Matrix

| Skill | Activate When | Do NOT Activate When | Upstream Required |
|-------|--------------|---------------------|-------------------|
| analyze-five-forces | Industry-level question, attractiveness, dynamics | Already have force assessment | None |
| profile-competitor | Specific competitor named, predict moves | No competitor identified | None |
| map-strategic-groups | Positioning, segmentation, mobility barriers | Single-competitor focus | None |
| diagnose-industry-type | Maturity, evolution, emerging/declining signals | Type already known and stated | None |
| select-generic-strategy | "What strategy?", cost vs differentiation | No industry context available | analyze-five-forces, map-strategic-groups |
| read-market-signals | Competitor announcement, pricing move, signal | No specific action to interpret | profile-competitor |
| analyze-market-entry | Enter new market, entry barriers, acquisition | Already operating in the market | analyze-five-forces |
| strategize-fragmented-industry | Diagnosed as fragmented | Not fragmented | diagnose-industry-type |
| strategize-emerging-industry | Diagnosed as emerging | Not emerging | diagnose-industry-type |
| strategize-declining-industry | Diagnosed as declining | Not declining | diagnose-industry-type |
| design-competitive-move | Plan attack/defense, respond to move | No specific action contemplated | profile-competitor, select-generic-strategy |
| audit-strategy-consistency | Evaluate coherence, post-formulation check | No strategy formulated yet | select-generic-strategy |

## Environment Assumptions

All skills assume:
- User can provide industry name and basic context
- Analysis is for a specific firm competing in the industry (not academic)
- Data may be incomplete — skills should note gaps rather than hallucinate

## Chaining Rules

1. Inspect skill output for downstream triggers (e.g., `diagnose-industry-type` outputs a type → route to type skill)
2. Only chain if the user's question warrants depth — don't run the full DAG for a simple question
3. If upstream data is missing, ask the user rather than skipping
4. Skip a skill if the user already provided its output as input
