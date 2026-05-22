---
name: read-market-signals
description: >
  Interpret competitor market signals using Porter's taxonomy. Use when asked to decode competitor announcements, pricing moves, cross-parries, or fighting brands.
---

# Read Market Signals

Classify and interpret a competitor's observed action as a market signal, assess whether it is a bluff or earnest commitment, and recommend a response.

## Input

1. **Observed action/announcement** -- what the competitor did or said, when, and through what medium.
2. **Competitor profile context** -- the competitor's goals, assumptions, capabilities, historical behavior, and market position (from a prior competitor-analysis skill or user-supplied notes).

## Output

1. Signal classification (which type from the taxonomy below).
2. Bluff vs. commitment assessment with supporting reasoning.
3. Recommended response (ignore, match, counter-signal, cross-parry, escalate).

## Procedure

1. **Identify the signal type.** Match the observed action to exactly one primary type in the taxonomy. Note if a secondary type also applies.
2. **Check the medium and timing.** Formal/broad-audience announcements establish public commitments that are hard to retract. Informal or narrow-audience signals (trade journals, sales-force chatter) may be tests of sentiment. Announcements made far in advance of action tend to be conciliatory.
3. **Apply bluff vs. commitment logic.** Use the classification rubric below.
4. **Analyze historical patterns.** Compare this signal against the competitor's prior behavior. Does it fit an established pattern (e.g., capacity announcements always at a certain utilization rate) or diverge from one?
5. **Assess divergence.** If the signal diverges from past goals or industry precedent, flag it as a potential major realignment requiring intensified monitoring.
6. **Determine severity and intent.** Map the signal onto the conciliation-aggression spectrum: Was the action less damaging than the worst the competitor could have done? If yes, lean toward conciliation. If it was maximally damaging, treat it as aggressive.
7. **Recommend response.** Factor in your own firm's position, cross-market exposure, and ability to counter-signal.

## Signal Taxonomy

| # | Signal Type | What It Looks Like | Primary Function |
|---|---|---|---|
| 1 | **Prior announcement of moves** | Formal communication that competitor will or will not take an action (plant, price, product) | Preemption, threat, test of sentiment, or conciliatory step |
| 2 | **After-the-fact announcement** | Public disclosure of results, sales figures, capacity data after they occurred | Ensure rivals notice; can inflate data to preempt or communicate commitment |
| 3 | **Public discussion of the industry** | Commentary on demand, pricing, capacity, cost trends | Expose assumptions; attempt to align industry on shared assumptions |
| 4 | **Discussion of own moves** | Competitor publicly explains the logic, cost, or difficulty of its move | Deter imitation, communicate commitment, or invite followership |
| 5 | **Tactics relative to what could have been done** | Choosing a move less damaging than the maximum feasible penalty | Signals conciliation when sub-optimal relative to narrow self-interest |
| 6 | **Manner of initial implementation** | Launching in a peripheral market, pricing at unusual times, targeting non-core segments | Differentiates penalty from industry-best-interest move |
| 7 | **Divergence from past goals** | Breaking historical focus (e.g., premium producer launching low-end product) | Indicates potential major realignment in goals or assumptions |
| 8 | **Divergence from industry precedent** | Actions that break established norms (discounting in a non-discount industry) | Usually an aggressive signal |
| 9 | **The fighting brand** | Introducing a brand that closely copies a threatening rival's product | Punish, warn, deter, or absorb the brunt of a competitive attack |
| 10 | **Cross-parry** | Responding to a competitor's move in a completely different geographic or product market | Signal displeasure indirectly; threaten retaliation without triggering destructive warfare in the contested market |
| 11 | **Private antitrust suit** | Filing a suit that can be dropped at any time | Mild signal of displeasure, harassment, or delay tactic |

## Bluff vs. Commitment Classification

Ask these questions in order:

1. **Would a surprise move have served the competitor better?** If yes, the announcement is likely conciliatory or a bluff, not preemptive.
2. **Are there lasting benefits from preemption?** If yes, treat the preemptive motive as a strong possibility.
3. **How formal and broad is the medium?** Formal press releases to broad audiences establish public commitments that are hard to retract. Narrow-audience signals are easier to walk back -- more likely a test or bluff.
4. **Is the disclosed data verifiable?** After-the-fact announcements of market share or capacity may inflate figures (e.g., quoting final planned capacity as initial capacity). Verify independently.
5. **Does the action diverge from narrow self-interest?** Behaving sub-optimally relative to what could maximally hurt rivals signals conciliation -- but could also be a sophisticated bluff.
6. **Has the competitor stressed the cost and difficulty of the move?** Emphasizing resources expended signals earnest long-run commitment.

## Cross-Parry Framework

A cross-parry occurs when Firm A moves in Market X and Firm B responds in Market Y (a different geography or product line) rather than countering directly. Interpretation:

- **Cross-parry in the initiator's core market**: severe warning. The defender is signaling willingness to escalate.
- **Cross-parry in a peripheral market**: milder deterrent. The defender hopes to avoid triggering hasty counterresponse but signals it will raise the ante if the initiator does not back off.
- **Divergent market shares amplify leverage**: if the cross-parrying firm has a smaller share in the contested market, a price cut there costs the larger-share initiator disproportionately more to match.
- **Maintaining a small position in cross-markets is a useful potential deterrent** even before any conflict arises.

## Historical Pattern Analysis

1. Search for recurring sequences: Do certain sales force activities always precede product changes? Do capacity announcements always occur at a specific utilization rate? Do price changes in the existing line always precede new product introductions?
2. Compare the current signal against these established patterns.
3. If the signal fits a known pattern, interpret it with higher confidence.
4. If the signal diverges from historical behavior, conduct a full competitor analysis to uncover economic or organizational reasons for the divergence before interpreting.

## Heuristics

- Every signal can be a bluff. Never treat any single signal as definitive without corroboration.
- The less damaging the chosen action relative to what was feasible, the more likely it is conciliatory.
- Fighting brands introduced with little push or support before any serious attack are warnings; those backed with full resources are offensive weapons. A fighting brand that copies a specific competitor's product is more effective discipline than a generalized new product.
- Private antitrust suits are the mildest signal of displeasure -- treat as a cross-parry equivalent.
- Too much attention to signals can itself be a distraction. Focus analysis time on signals that would materially change your strategic choices.

## Failure Modes

- **Mirror-imaging**: assuming the competitor thinks like you. Always ground interpretation in their goals and assumptions, not yours.
- **Over-reading a single signal**: one data point is not a pattern. Corroborate with historical behavior and multiple signal types.
- **Ignoring the medium**: treating a narrow-audience trial balloon the same as a formal public commitment.
- **Neglecting divergence risk**: assuming historical patterns will always hold. Changed economics or leadership can break patterns.
- **Confusing conciliation with weakness**: a sub-optimal move may be an invitation to cooperate, not a sign the competitor cannot do more.

## Output Template

```
## Signal Reading: [Competitor Name] -- [Action Summary]

**Signal type**: [from taxonomy]
**Medium & timing**: [where announced, when, how far in advance of action]
**Bluff vs. commitment**: [assessment + reasoning from classification rubric]
**Historical pattern fit**: [consistent / divergent / insufficient data]
**Severity**: [conciliatory / neutral / aggressive]
**Recommended response**: [ignore / match / counter-signal / cross-parry / escalate]
**Rationale**: [1-3 sentences linking the above to recommended action]
```

## Worked Example

**Scenario**: AcmeCorp, a premium-segment manufacturer, announces in a formal press release that it will build a new plant with capacity equal to 100% of projected industry demand growth. AcmeCorp has historically only added capacity at 90%+ utilization. Current utilization is 72%.

1. **Signal type**: Prior announcement of moves (Type 1), with divergence from past goals (Type 7) since the announcement occurs well below the historical 90% utilization trigger.
2. **Medium & timing**: Formal press release to broad audience -- establishes a public commitment that is hard to retract.
3. **Bluff vs. commitment**: The formal, broad-audience medium suggests earnest commitment. However, the divergence from the historical 90% utilization pattern is suspicious. A surprise groundbreaking would have been more preemptive; the advance announcement suggests either a desire to deter rivals (preemption) or a test of sentiment. Check whether AcmeCorp has lasting benefits from preemption (e.g., locking up contractor capacity, customer commitments). If yes, treat as earnest preemption. If not, the early timing and utilization divergence suggest a possible bluff to scare off rival capacity additions.
4. **Historical pattern fit**: Divergent -- capacity has never been announced below 90% utilization.
5. **Severity**: Aggressive (sized to absorb all industry growth).
6. **Recommended response**: Do not immediately cancel own capacity plans. Monitor for ground-breaking activity and contractor commitments within 90 days. If no physical action follows, reclassify as bluff and proceed with own expansion. Consider a counter-signal: publicly discuss your own capacity plans to test AcmeCorp's reaction.
