# Workflows Catalog

## Primary DAG

```
                    ┌─→ select-generic-strategy ─→ design-competitive-move
analyze-five-forces─┤                            ↗
                    └─→ analyze-market-entry     audit-strategy-consistency
                                                  ↑
map-strategic-groups ──→ select-generic-strategy ──┘

profile-competitor ──→ read-market-signals
                   └─→ design-competitive-move

diagnose-industry-type ──→ strategize-fragmented-industry
                       ──→ strategize-emerging-industry
                       ──→ strategize-declining-industry
```

### Parallelizable Operations
- `analyze-five-forces` + `profile-competitor` + `map-strategic-groups` + `diagnose-industry-type` (all Tier 1, no deps)
- `read-market-signals` can run alongside `select-generic-strategy` (different inputs)

## Standalone Workflows

### 1. Quick Industry Check
**Entry:** "How attractive is this industry?"
**Chain:** `analyze-five-forces` → `diagnose-industry-type` → (route to type-specific skill if applicable)
**Output:** Industry attractiveness + evolutionary stage + type-specific strategy if warranted

### 2. Competitor Deep Dive
**Entry:** "Analyze [competitor]"
**Chain:** `profile-competitor` → `read-market-signals` (if recent actions exist)
**Output:** Full competitor profile + signal interpretation

### 3. Should We Enter?
**Entry:** "Should we enter [market]?"
**Chain:** `analyze-five-forces` → `analyze-market-entry`
**Output:** Industry structure + go/no-go + entry mechanism

### 4. What Move?
**Entry:** "How should we compete against [competitor]?"
**Chain:** `profile-competitor` → `select-generic-strategy` → `design-competitive-move`
**Output:** Competitor profile + strategy selection + specific move design

### 5. Full Strategic Audit
**Entry:** "Full competitive analysis"
**Chain:** `analyze-five-forces` → `map-strategic-groups` → `select-generic-strategy` → `audit-strategy-consistency`
**Output:** Complete industry + positioning + strategy + consistency check
