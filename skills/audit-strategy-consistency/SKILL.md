---
name: audit-strategy-consistency
description: >
  Audit a competitive strategy for internal consistency using Porter's tests. Use when evaluating whether a strategy hangs together, after formulating strategy, or when diagnosing strategic drift.
---

# Audit Strategy Consistency

Run Porter's Figure 1-3 consistency tests against a firm's competitive strategy to determine whether goals and policies form a coherent, implementable whole.

## Input

The firm's current competitive strategy: explicit goals (financial, market position, social) and key operating policies across each functional area. Typically produced by upstream skills (e.g., `formulate-strategy`). If not available, extract from the user's description.

## Output

- Pass/fail verdict per test question, with supporting evidence or gap identified
- Category-level summary (Internal Consistency, Environmental Fit, Resource Fit, Communication & Implementation)
- Overall consistency verdict: CONSISTENT, PARTIALLY CONSISTENT, or INCONSISTENT
- Priority list of inconsistencies requiring resolution

## Procedure

1. **Inventory the strategy.** List the firm's stated goals and key operating policies. If goals or policies are vague, flag this before proceeding -- the tests require specificity.
2. **Run Internal Consistency tests.** Evaluate each question below against the stated goals and policies.
3. **Run Environmental Fit tests.** Cross-reference goals/policies against industry analysis (five forces, opportunities, threats, societal factors).
4. **Run Resource Fit tests.** Compare goals/policies against the firm's resources relative to competitors.
5. **Run Communication & Implementation tests.** Assess whether the strategy can actually be executed by the people responsible.
6. **Synthesize.** Aggregate pass/fail results into a category summary and overall verdict. Identify the most critical inconsistencies.

## Tests of Consistency (Porter, Figure 1-3)

### A. Internal Consistency

1. Are the goals mutually achievable?
2. Do the key operating policies address the goals?
3. Do the key operating policies reinforce each other?

### B. Environmental Fit

4. Do the goals and policies exploit industry opportunities?
5. Do the goals and policies deal with industry threats (including the risk of competitive response) to the degree possible with available resources?
6. Does the timing of the goals and policies reflect the ability of the environment to absorb the actions?
7. Are the goals and policies responsive to broader societal concerns?

### C. Resource Fit

8. Do the goals and policies match the resources available to the company relative to competitors?
9. Does the timing of the goals and policies reflect the organization's ability to change?

### D. Communication and Implementation

10. Are the goals well understood by the key implementers?
11. Is there enough congruence between the goals and policies and the values of the key implementers to insure commitment?
12. Is there sufficient managerial capability to allow for effective implementation?

During synthesis, consult `reference.md` for Porter's heuristics on consistency; before finalizing, check its failure modes.

## Output Template

```
## Strategy Consistency Audit: [Firm/Business Unit]

### Strategy Summary
- Goals: [list]
- Key Operating Policies: [list by functional area]

### Test Results

#### A. Internal Consistency
| # | Test | Verdict | Evidence |
|---|------|---------|----------|
| 1 | Goals mutually achievable? | PASS/FAIL | [reasoning] |
| 2 | Policies address goals? | PASS/FAIL | [reasoning] |
| 3 | Policies reinforce each other? | PASS/FAIL | [reasoning] |

#### B. Environmental Fit
| # | Test | Verdict | Evidence |
|---|------|---------|----------|
| 4 | Exploit opportunities? | PASS/FAIL | [reasoning] |
| 5 | Deal with threats? | PASS/FAIL | [reasoning] |
| 6 | Timing vs. environment? | PASS/FAIL | [reasoning] |
| 7 | Responsive to societal concerns? | PASS/FAIL | [reasoning] |

#### C. Resource Fit
| # | Test | Verdict | Evidence |
|---|------|---------|----------|
| 8 | Match available resources? | PASS/FAIL | [reasoning] |
| 9 | Timing vs. change capacity? | PASS/FAIL | [reasoning] |

#### D. Communication & Implementation
| # | Test | Verdict | Evidence |
|---|------|---------|----------|
| 10 | Goals understood? | PASS/FAIL | [reasoning] |
| 11 | Congruent with values? | PASS/FAIL | [reasoning] |
| 12 | Sufficient capability? | PASS/FAIL | [reasoning] |

### Overall Verdict: [CONSISTENT / PARTIALLY CONSISTENT / INCONSISTENT]

### Priority Inconsistencies
1. [Most critical gap + which test failed]
2. [Next most critical]
```

## Worked Example

**Firm:** Regional grocery chain pursuing both cost leadership (goal: lowest prices in market) and premium organic selection (goal: widest organic assortment).

**Test 1 -- Goals mutually achievable?** FAIL. Lowest-price positioning requires cost minimization across procurement and operations. Widest organic assortment requires premium supplier relationships and higher SKU complexity, which drives costs up. The goals work against each other.

**Test 3 -- Policies reinforce each other?** FAIL. Procurement policy targets lowest-cost suppliers, but merchandising policy mandates premium organic brands. These policies create internal conflict in buyer decision-making.

**Test 5 -- Deal with threats?** FAIL. Competitors (Whole Foods, Aldi) each own one positioning clearly. Straddling invites competitive response from both directions with no defensible position.

**Test 8 -- Match available resources?** FAIL. The firm lacks the scale for cost leadership (regional vs. national chains) and the brand equity for premium organic positioning simultaneously.

**Overall Verdict:** INCONSISTENT. The strategy attempts to straddle two generic strategies. Resolution requires choosing one position or defining a focused segment where both goals are achievable (e.g., "affordable organic for families" in a specific metro area).
