---
name: map-strategic-groups
description: >
  Map strategic groups within an industry using Porter's framework. Use when asked to segment competitors, identify positioning opportunities, or analyze mobility barriers.
---

## Purpose

Construct a strategic group map of an industry to reveal mobility barriers, inter-group rivalry dynamics, and positioning opportunities by plotting competitors along the two most structurally significant strategic dimensions.

## Input/Output Contract

- **Accepts:** A list of competitors (or an industry name to research) with information about their strategic approaches, plus optionally a specific strategic question.
- **Produces:** Strategic group map (ASCII 2D grid), mobility barrier assessment between groups, per-group structural analysis, and positioning opportunity insights.
- **Passes to:** `select-generic-strategy` (to choose a strategy within the identified group), `design-competitive-move` (to plan movement between groups or defend position).

## Procedure

1. **Profile each competitor** across all 13 strategic dimensions (see catalog below).
2. **Select two dimensions** for the map axes using the dimension selection criteria.
3. **Plot competitors** on the 2D grid; cluster firms with similar positions into named groups.
4. **Size each group** proportionally by combined market share or revenue.
5. **Assess mobility barriers** between each pair of adjacent groups.
6. **Analyze each group** for rivalry intensity, bargaining power, and substitute vulnerability.
7. **Identify positioning opportunities** -- gaps, marginal groups, trends enabling movement.
8. **Synthesize** strategic implications for the focal firm.

## Strategic Dimensions Catalog

Profile every competitor along these dimensions (Porter's exhaustive list):

| # | Dimension | What to Assess |
|---|-----------|---------------|
| 1 | **Specialization** | Width of product line, target customer segments, geographic markets served |
| 2 | **Brand identification** | Degree of reliance on branding (via advertising, sales force, etc.) vs. price competition |
| 3 | **Push vs. pull** | Emphasis on direct consumer brand identification vs. relying on distribution channels to sell |
| 4 | **Channel selection** | Company-owned channels, specialty outlets, or broad-line outlets |
| 5 | **Product quality** | Raw materials, specifications, adherence to tolerances, features |
| 6 | **Technological leadership** | Pioneer vs. follower/imitator (note: tech leadership and quality do not necessarily go together) |
| 7 | **Vertical integration** | Extent of forward and backward integration -- captive distribution, owned retail, in-house service |
| 8 | **Cost position** | Investment in cost-minimizing facilities and equipment for manufacturing and distribution |
| 9 | **Service** | Ancillary services: engineering assistance, in-house service network, credit |
| 10 | **Price policy** | Relative price position in the market (related to but distinct from cost position and quality) |
| 11 | **Leverage** | Amount of financial leverage and operating leverage |
| 12 | **Relationship with parent company** | Objectives, shared resources, and constraints from being part of a conglomerate, vertical chain, or foreign subsidiary |
| 13 | **Relationship with home/host government** | Regulatory constraints or assistance from home and host governments |

## Dimension Selection Criteria

When choosing which two dimensions to use as map axes, apply Porter's three rules:

1. **Determine key barriers:** Select dimensions that determine the most critical mobility barriers in the industry. Example: in soft drinks, brand identification and distribution channels are the key barriers and thus the best axes.
2. **Avoid correlated variables:** Do not select dimensions that move together. If all highly differentiated firms also have broad product lines, using both yields no insight. Choose dimensions that reflect the diversity of strategic combinations.
3. **Non-continuous variables are valid:** Axes do not have to be continuous or monotonic. Discrete categories work (e.g., "servicing dealers / mass merchandisers / private label" as a channel axis).

## Mapping Instructions

1. Draw a 2D grid with the two selected dimensions as axes.
2. Position each competitor on the grid based on its profile on those two dimensions.
3. Draw circles around clusters of firms occupying similar positions -- these are strategic groups.
4. Size each circle proportional to the group's combined market share.
5. Label each group with a descriptive name reflecting its shared strategy.
6. If a single map misses important strategic variation, construct multiple maps using different axis pairs.

## Mobility Barrier Assessment

Mobility barriers are the economic factors that deter firms from shifting strategy to move from one group to another. They are the same factors as entry barriers -- economies of scale, capital requirements, product differentiation, switching costs, absolute cost advantages, access to distribution -- but applied to protect specific strategic positions within the industry.

For each pair of adjacent groups, assess:
- What investments would a firm need to make to move from Group A to Group B?
- Which barrier sources (scale, differentiation, capital, cost advantages, distribution access) are most significant?
- Are barriers symmetric or asymmetric between the two groups?
- How do accumulated experience and brand identification create barriers?

## Per-Group Analysis

For each strategic group, assess the five competitive forces at the group level:

1. **Rivalry intensity** -- determined by four factors:
   - Market interdependence: how much do groups' customer targets overlap?
   - Product differentiation: how distinct are the groups' offerings?
   - Number and relative size of groups: more equal-sized groups means more rivalry.
   - Strategic distance: how fundamentally different are the competitive approaches? Greater distance intensifies rivalry when groups compete for the same customers.

2. **Bargaining power with suppliers/buyers** -- groups differ because:
   - Their strategies yield differing vulnerability to common suppliers or buyers.
   - Their strategies require dealing with entirely different suppliers or buyers with different leverage levels.

3. **Substitute vulnerability** -- which groups' strategies expose them most to substitutes from outside the industry?

## Positioning Opportunities

Formulating competitive strategy is the choice of which strategic group to compete in. This choice involves finding the best trade-off between a group's profit potential and the firm's cost of entering it. Identify opportunities using Porter's four categories:

1. **Create a new strategic group** -- technological changes or structural evolution may open positions no firm currently occupies. Even without external stimuli, a visionary firm may perceive a favorably situated group not seen by competitors.
2. **Shift to a more favorably situated group** -- move to a group with stronger mobility barriers, less rivalry exposure, or better bargaining position. Consider sequenced entry: enter a low-barrier group first to accumulate capital, brand recognition, or experience, then leap to the ultimate target group.
3. **Strengthen the structural position of the existing group** -- reinforce mobility barriers that protect your current group.
4. **Strengthen your position within your group** -- improve implementation relative to group peers.

Also assess:
- **Gaps on the map** where no group exists -- could a viable strategy occupy that space?
- **Marginal groups** with weak barriers and poor structural position -- candidates for disruption.
- **Industry trends** that may lower mobility barriers between groups or create new strategic positions.

## Heuristics

- The profit potential of a firm is a function of (a) the industry's common structural characteristics, (b) the structural characteristics of its strategic group (mobility barriers, bargaining power, substitute exposure, rivalry from other groups), and (c) the firm's position within its group.
- Structural strengths (mobility barriers, bargaining position) are relatively stable and difficult to overcome; implementational strengths (managerial ability, execution) are more ephemeral.
- When industry structure is unchanging, the cost of overcoming mobility barriers to join an occupied group may eliminate the benefits. Significant repositioning gains come when industry evolution lowers the cost of shifting.
- Sequenced entry lowers total cost and risk by segmenting the investment: enter via reversible investments first (e.g., private label production), then advance to groups requiring irreversible investments (advertising, R&D).

## Failure Modes

1. **Choosing correlated dimensions** -- selecting axes that move together collapses the map into a diagonal line with no strategic insight.
2. **Making every firm its own group** -- over-segmenting destroys the analytical power of grouping; cluster firms with genuinely similar strategies.
3. **Ignoring mobility barriers** -- mapping groups without assessing what prevents movement between them misses the core structural insight.
4. **Using only one map** -- a single pair of axes may miss important strategic variation; consider multiple maps.
5. **Confusing quality with technological leadership** -- Porter explicitly warns these do not necessarily go together.
6. **Ignoring parent company and government relationships** -- these dimensions are easy to overlook but can be decisive in some industries.

## Output Format

```markdown
## Strategic Group Map: [Industry]

### Axes Selected
- **X-axis:** [Dimension] -- rationale: [why this determines key mobility barriers]
- **Y-axis:** [Dimension] -- rationale: [why this determines key mobility barriers]

### Map

            High |  [Group C]        [Group D]
                 |    (15%)            (25%)
  [Y-Dimension] |
                 |  [Group A]        [Group B]
            Low  |    (35%)            (25%)
                 +-----------------------------
                   Low                    High
                        [X-Dimension]

### Group Profiles
#### Group A: [Name]
- **Members:** Firm 1, Firm 2, Firm 3
- **Shared strategy:** [description across key dimensions]
- **Mobility barriers protecting this group:** [list]
- **Rivalry exposure:** [high/medium/low + rationale]
- **Bargaining position:** Suppliers [assessment], Buyers [assessment]
- **Substitute vulnerability:** [assessment]

[Repeat for each group]

### Mobility Barriers Between Groups
| From \ To | Group A | Group B | Group C | Group D |
|-----------|---------|---------|---------|---------|
| Group A   | --      | [barrier] | [barrier] | [barrier] |
| ...       |         |         |         |         |

### Positioning Opportunities
1. [Opportunity type]: [description]
2. ...

### Strategic Implications for [Focal Firm]
- Current group: [which group]
- Recommended action: [stay/move/create new group]
- Rationale: [structural analysis]
```

## Example Execution

**Industry:** U.S. Chain Saw Industry (Porter's example)

**Axes:** Brand identification (Y) vs. Channel selection (X: servicing dealers / mass merchandisers / private label)

**Groups identified:**
- **Group A (Professional-grade):** Stihl, Husqvarna -- high brand ID, servicing dealers, high quality, narrow specialization. Protected by brand loyalty, dealer relationships, and R&D investment.
- **Group B (Mass-market branded):** Firms selling through mass merchandisers with moderate brand identification. Lower mobility barriers than Group A.
- **Group C (Private label):** Firms producing for private label accounts -- low brand ID, compete on cost position. Low mobility barriers to enter but high barriers to exit into branded groups (requires massive advertising investment).

**Key insight:** Moving from private label (Group C) to professional-grade (Group A) requires overcoming barriers in brand identification, dealer network development, and product quality -- a candidate for sequenced entry through Group B first.
