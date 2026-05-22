# Porter Competitive Strategy Skills

**Turn competitive strategy from abstract theory into structured analysis.**

12 executable skills + 1 orchestrator extracted from Michael Porter's *Competitive Strategy* — the foundational text on industry analysis and competitive positioning. Every skill was sense-checked against the original book via NotebookLM. Every sub-factor, checklist, and decision tree comes from Porter's own language, not summaries or interpretations.

Ask your agent to "analyze this industry" and get a structured five forces assessment with 32 sub-factors rated. Ask "what move should we make?" and get a commitment framework with retaliation predictions. Ask "are we stuck in the middle?" and get a diagnostic checklist with organizational requirements you're missing.

---

## Get started

```
/orchestrate-porter-strategy
```

The orchestrator detects what you're asking and routes to the right skill(s). Or invoke any skill directly:

```
/analyze-five-forces
/profile-competitor
/select-generic-strategy
```

---

## The 12 skills

### Tier 1 — Entry points (no dependencies)

| Skill | What it does | Porter source |
|-------|-------------|---------------|
| `/analyze-five-forces` | Assess industry structure across 32 sub-factors (8 entry barriers, 8 rivalry drivers, 7 buyer power factors, 6 supplier power factors, 3 substitute indicators), identify governing forces, rate overall profit potential | Ch 1 |
| `/profile-competitor` | Build a four-component competitor profile (future goals, assumptions, current strategy, capabilities), generate a response profile predicting satisfaction, likely moves, vulnerabilities, and retaliation triggers | Ch 3 |
| `/map-strategic-groups` | Plot competitors across 13 strategic dimensions, select optimal axes, assess mobility barriers between groups, analyze per-group rivalry and bargaining power differences | Ch 7 |
| `/diagnose-industry-type` | Classify an industry as emerging, fragmented, transitioning to maturity, or declining using Porter's 14 evolutionary processes, then route to the appropriate industry-type strategy skill | Ch 8–12 |

### Tier 2 — Build on Tier 1 outputs

| Skill | What it does | Porter source |
|-------|-------------|---------------|
| `/select-generic-strategy` | Evaluate cost leadership, differentiation, and focus against your situation. Full requirements tables (skills, org arrangements, control systems), risk profiles, and a stuck-in-the-middle diagnostic | Ch 2 |
| `/read-market-signals` | Interpret competitor actions using Porter's 11-type signal taxonomy. Classify bluff vs. commitment, decode cross-parries and fighting brands, analyze historical behavior patterns | Ch 4 |
| `/analyze-market-entry` | Go/no-go entry analysis with barrier cost estimation, 7 generic entry mechanisms, incumbent retaliation modeling, sequenced entry assessment, and acquisition framework | Ch 16 |
| `/strategize-fragmented-industry` | Porter's 5-step process for fragmented industries. 11 fragmentation causes with overcomability assessment, 9 coping strategies, consolidation vs. cope recommendation | Ch 9 |
| `/strategize-emerging-industry` | Scenario-based forecasting, shape vs. adapt decision, pioneer vs. follower timing, 8 structural characteristics, shifting barrier analysis | Ch 10 |
| `/strategize-declining-industry` | End-game strategy selection using the 2x2 matrix (industry structure vs. firm strengths). 4 strategies (Leadership, Niche, Harvest, Divest) with hospitability assessment and exit barrier analysis | Ch 12 |

### Tier 3 — Requires competitor profile + strategy selection

| Skill | What it does | Porter source |
|-------|-------------|---------------|
| `/design-competitive-move` | Design offensive or defensive moves. Cooperative vs. threatening classification, mixed motives exploitation, commitment credibility framework, focal points, deny-the-base defense | Ch 5 |
| `/audit-strategy-consistency` | Test a strategy against Porter's 12 consistency checks across internal consistency, environmental fit, resource fit, and communication/implementation | Intro |

### Orchestrator

| Skill | What it does |
|-------|-------------|
| `/orchestrate-porter-strategy` | Detect intent, route to the right skill(s), chain outputs, accumulate context. 5 pre-built workflow shortcuts for common analyses |

---

## Pick your scenario

**"How attractive is this industry?"**
```
/analyze-five-forces
```
Walks through all 5 forces with every sub-factor Porter identifies. Produces a rated assessment with the governing force highlighted and strategic implications.

**"What will our competitor do next?"**
```
/profile-competitor
```
Builds a four-component profile, detects blind spots via assumption analysis, and predicts responses to your potential moves.

**"Should we enter this market?"**
```
/analyze-market-entry
```
Estimates true entry cost (not just visible investments), models incumbent retaliation, evaluates 7 entry mechanisms, and considers sequenced entry to lower risk.

**"We're in a crowded market with no dominant player"**
```
/strategize-fragmented-industry
```
Diagnoses why the industry is fragmented, whether consolidation is feasible, and which of 9 coping strategies fits your position.

**"Is our strategy coherent?"**
```
/audit-strategy-consistency
```
Runs 12 consistency tests from Porter's Figure 1-3. Flags where goals contradict policies, resources don't match ambitions, or timing is off.

**"What competitive move should we make?"**
```
/design-competitive-move
```
Designs a move that exploits mixed motives — where the competitor's rational response would hurt their own broader goals. Includes commitment requirements and escalation risk assessment.

---

## Workflow shortcuts

The orchestrator includes 5 pre-built chains for common analyses:

| Workflow | Chain | Trigger |
|----------|-------|---------|
| Quick Industry Check | five-forces → diagnose-type → (type strategy) | "Analyze this industry" |
| Competitor Deep Dive | profile-competitor → read-signals | "Analyze [competitor]" |
| Should We Enter? | five-forces → market-entry | "Should we enter [market]?" |
| What Move? | profile-competitor → generic-strategy → competitive-move | "How should we compete?" |
| Full Strategic Audit | five-forces → strategic-groups → generic-strategy → consistency | "Full competitive analysis" |

---

## What's in the box

```
porter-strategy-skills/
├── skills/
│   ├── orchestrate-porter-strategy/SKILL.md
│   ├── analyze-five-forces/SKILL.md
│   ├── profile-competitor/SKILL.md
│   ├── map-strategic-groups/SKILL.md
│   ├── diagnose-industry-type/SKILL.md
│   ├── select-generic-strategy/SKILL.md
│   ├── read-market-signals/SKILL.md
│   ├── analyze-market-entry/SKILL.md
│   ├── strategize-fragmented-industry/SKILL.md
│   ├── strategize-emerging-industry/SKILL.md
│   ├── strategize-declining-industry/SKILL.md
│   ├── design-competitive-move/SKILL.md
│   └── audit-strategy-consistency/SKILL.md
├── heuristics/catalog.md      ← 57 Porter-derived rules of thumb
├── failures/catalog.md        ← 65 failure modes with root causes
├── workflows/catalog.md       ← DAG + 5 standalone workflows
├── routing/context-rules.md   ← Full activation matrix
└── references/source-summary.md ← Chapter coverage + known gaps
```

Each skill includes:
- Step-by-step procedure using Porter's exact language
- Exhaustive sub-factor checklists (not summaries)
- Decision logic for synthesizing findings into recommendations
- Heuristics — rules of thumb Porter gives for quick judgment calls
- Failure modes — what goes wrong and how to detect it
- Structured output template
- Worked example showing input → output

---

## What Porter covers that this plugin doesn't (yet)

| Gap | Porter Chapter | Why it's not here |
|-----|---------------|-------------------|
| Global industry strategy | Ch 13 | Multi-domestic vs. global competition framework — could warrant a `strategize-global-industry` skill |
| Vertical integration analysis | Ch 14 | Make-vs-buy, quasi-integration, tapered integration — could be its own skill |
| Capacity expansion | Ch 15 | Preemptive capacity, overbuilding dynamics — could fold into `design-competitive-move` |
| Buyer/supplier strategy | Ch 6 | Strategy toward specific buyers/suppliers beyond the five forces assessment |

---

## Installation

### Cursor

```
/add-plugin https://github.com/gnurio/porter-strategy-skills
```

### Claude Code

Clone into your skills directory:

```bash
git clone https://github.com/gnurio/porter-strategy-skills.git ~/.claude/skills/porter-strategy
```

### Cowork

Add the plugin URL in your Cowork workspace settings, or clone the repo and point your workspace to the `skills/` directory.

---

## Source fidelity

Every skill was built using this protocol:

1. **NotebookLM sense-check** — queried the full Porter PDF for every sub-factor, checklist, and procedure the skill covers
2. **Write** — structured the skill using the NLM response as ground truth
3. **Validation spot-check** — ran a second query to verify a specific detail (e.g., "Does Porter treat government as a sixth force?") and fixed any discrepancies

This matters because strategy frameworks get watered down through summarization. These skills preserve Porter's actual analytical procedures — the 8 entry barrier sub-factors, the 4-question competitor response profile, the 14 evolutionary processes — not MBA-textbook paraphrases.

---

## License

[CC BY 4.0](LICENSE) — free to use, share, and adapt with attribution.

Built by [George Nurijanian](https://github.com/gnurio) · [prodmgmt.world](https://prodmgmt.world)
