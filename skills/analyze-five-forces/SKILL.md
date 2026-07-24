---
name: analyze-five-forces
description: >
  Analyze industry structure using Porter's Five Forces. Use when asked to assess industry attractiveness, competitive dynamics, profit potential, or structural threats.
---

# Analyze Five Forces

**Purpose:** Diagnose the structural forces that determine industry competition and long-run profit potential, using Porter's exact framework from *Competitive Strategy*.

## Input

- **Required:** Industry name or description
- **Optional:** Specific data on competitors, suppliers, buyers, substitutes, or entrants

## Output

1. Force-by-force assessment with sub-factor ratings
2. Overall industry attractiveness (profit potential)
3. Identification of the governing force(s)
4. Strategic implications

## Procedure

For each force, assess EVERY sub-factor below. Rate each sub-factor High / Medium / Low for its contribution to force strength, then rate the overall force.

### Force 1: Threat of Entry

Assess the barriers to entry that determine how easily new firms can enter. Higher barriers = lower threat.

| Sub-factor | What to assess |
|---|---|
| **Economies of scale** | Do unit costs decline significantly with volume across manufacturing, R&D, marketing, distribution? Must entrants come in at large scale or accept cost disadvantage? |
| **Product differentiation** | Do incumbents have strong brand identification and customer loyalty? Must entrants spend heavily to overcome? |
| **Capital requirements** | How large is the financial investment to compete, especially unrecoverable up-front costs (advertising, R&D)? |
| **Switching costs** | Do buyers face one-time costs when changing from one supplier to another? |
| **Access to distribution channels** | Must entrants persuade channels to accept their products through price breaks, advertising allowances, etc.? Are channels tied up? |
| **Cost disadvantages independent of scale** | Do incumbents hold proprietary technology, favorable raw material access, favorable locations, government subsidies, or learning/experience curve advantages? |
| **Government policy** | Does government limit or foreclose entry via licensing, pollution standards, product safety regulations, or raw material restrictions? |
| **Expected retaliation** | Do incumbents have a history of vigorous retaliation? Do they hold excess resources to fight back? Is industry growth slow enough that entrants must take share? |

### Force 2: Intensity of Rivalry Among Existing Competitors

Rivalry takes the form of price competition, advertising battles, product introductions, and increased customer service. Firms are mutually dependent -- moves incite retaliation.

| Sub-factor | What to assess |
|---|---|
| **Numerous or equally balanced competitors** | Are there many firms, or few firms of similar size and resources? Neither can dominate. |
| **Slow industry growth** | Does slow growth turn competition into a market-share fight rather than expansion? |
| **High fixed or storage costs** | Do high fixed costs create pressure to fill capacity, leading to price cutting? |
| **Lack of differentiation or switching costs** | Is the product a commodity? Can buyers switch freely, making choice based on price and service? |
| **Capacity augmented in large increments** | Must capacity be added in large blocks, disrupting supply-demand balance and causing overcapacity? |
| **Diverse competitors** | Do competitors differ in strategies, origins, personalities, and parent relationships? Foreign firms, owner-operators, and firms using the market as an outlet for excess capacity increase volatility. |
| **High strategic stakes** | Do firms have strong motives (corporate strategy, global prestige) to succeed here, making them willing to sacrifice profitability? |
| **High exit barriers** | Do specialized assets, fixed costs of exit, strategic interrelationships, emotional barriers, or government restrictions keep firms competing even with poor returns? |

### Force 3: Bargaining Power of Buyers

Buyers compete with the industry by forcing down prices, bargaining for higher quality or more services, and playing competitors against each other.

| Sub-factor | What to assess |
|---|---|
| **Buyer concentration or large volume purchases** | Do buyers purchase large quantities relative to seller sales? Especially powerful when seller has high fixed costs. |
| **Products are standard or undifferentiated** | Can buyers always find alternative suppliers and play them against each other? |
| **Buyer faces few switching costs** | Is the buyer free to change suppliers without penalty? |
| **Buyer earns low profits** | Do low profits create aggressive incentive to lower purchasing costs? |
| **Threat of backward integration** | Can the buyer credibly manufacture the product itself? |
| **Product is unimportant to buyer's quality** | Is the purchased input non-critical to the buyer's own product quality or performance? Makes buyer more price-sensitive. |
| **Buyer has full information** | Does the buyer know actual demand, market prices, and supplier costs? Full information yields maximum leverage. |

### Force 4: Bargaining Power of Suppliers

Mirror image of buyer power. A supplier group is powerful when:

| Sub-factor | What to assess |
|---|---|
| **Supplier concentration** | Is the supplier group dominated by a few companies and more concentrated than the industry it sells to? |
| **Availability of substitutes** | Must the supplier contend with substitute products? Lack of substitutes increases power. |
| **Industry is not an important customer** | Is the purchasing industry a small fraction of the supplier's sales? Suppliers exert more power when not dependent on the industry. |
| **Supplier's product is important input** | Is the input critical to the buyer's manufacturing process or product quality? Especially if non-storable. |
| **Differentiation or switching costs** | Is the supplier's product differentiated or does it create buyer lock-in? Cuts off ability to play suppliers against each other. |
| **Threat of forward integration** | Can the supplier credibly enter the buyer's industry? Checks the industry's ability to demand better terms. |

### Force 5: Threat of Substitute Products

Substitutes are products that can perform the same function as the industry's product. Identifying them may require looking at businesses seemingly far removed from the industry.

| Sub-factor | What to assess |
|---|---|
| **Price-performance of substitutes** | Does a substitute offer a superior price-performance tradeoff? Places a ceiling on industry prices. |
| **Switching costs to substitutes** | How costly or difficult is it for buyers to switch to the substitute? |
| **Buyer propensity to substitute** | Are buyers actively exploring or adopting alternatives? |

### Cross-cutting: Government and Technology

Porter explicitly rejects treating government or technology as a separate sixth force. Instead: "It is usually more illuminating to consider how government affects competition through the five competitive forces than to consider it as a force in and of itself." Analyze government's impact under each force (entry barriers, buyer/supplier power as government buyer/supplier, rivalry via regulation, substitutes via subsidies/standards). Same for technology.

## Scoring Guidance

1. Rate each sub-factor: **High** (strongly increases force strength), **Medium**, or **Low** (weak/absent)
2. Rate each force overall: **High** (erodes profits), **Medium**, **Low** (favorable to incumbents)
3. No mechanical weighting -- use judgment about which sub-factors matter most in context

## Synthesis

1. **Identify the governing force(s):** "The strongest force or forces are governing and become crucial from the point of view of strategy formulation." A single dominant force can cap profitability regardless of other conditions.
2. **Assess overall profit potential:** The collective strength of the five forces determines long-run return on invested capital. Strong forces = low profit potential; weak forces = attractive industry.
3. **Strategic positioning:** Can the firm defend against the forces, influence them in its favor, or anticipate shifts and exploit change before rivals recognize it?

During synthesis, consult `reference.md` for Porter's heuristics on structural analysis; before finalizing, check its failure modes.

## Output Template

```markdown
# Five Forces Analysis: [Industry]

## 1. Threat of Entry: [High/Medium/Low]
- Economies of scale: [rating] -- [1-2 sentence justification]
- Product differentiation: [rating] -- [justification]
- Capital requirements: [rating] -- [justification]
- Switching costs: [rating] -- [justification]
- Access to distribution: [rating] -- [justification]
- Cost disadvantages independent of scale: [rating] -- [justification]
- Government policy: [rating] -- [justification]
- Expected retaliation: [rating] -- [justification]

## 2. Rivalry Among Competitors: [High/Medium/Low]
[Same pattern for all sub-factors]

## 3. Bargaining Power of Buyers: [High/Medium/Low]
[Same pattern for all sub-factors]

## 4. Bargaining Power of Suppliers: [High/Medium/Low]
[Same pattern for all sub-factors]

## 5. Threat of Substitutes: [High/Medium/Low]
[Same pattern for all sub-factors]

## Synthesis
- **Governing force(s):** [which force(s) dominate and why]
- **Overall profit potential:** [High/Medium/Low] -- [explanation]
- **Strategic implications:** [2-3 actionable observations about positioning]
```

## Worked Example: U.S. Craft Beer Industry

**1. Threat of Entry: Medium**
- Economies of scale: Low -- small-batch production viable; distribution scale matters more
- Product differentiation: High -- strong brand loyalty, local identity, taproom culture
- Capital requirements: Medium -- microbrewery setup ~$500K-2M; large-scale much higher
- Switching costs: Low -- consumers switch brands easily
- Access to distribution: High -- three-tier system constrains access; shelf space is scarce
- Cost disadvantages independent of scale: Low -- recipes not proprietary; ingredients commodity
- Government policy: Medium -- federal/state licensing, labeling, distribution laws
- Expected retaliation: Low -- incumbents rarely retaliate against small entrants

**2. Rivalry: High**
- Numerous competitors: High -- 9,000+ breweries; highly fragmented
- Slow growth: Medium -- growth slowing after boom years
- High fixed costs: Medium -- brewing equipment utilization pressure
- Lack of differentiation: Low -- products are differentiated by style, brand, locality
- Diverse competitors: High -- mix of large nationals, regionals, micros, brewpubs

**3. Buyer Power: Medium**
- Distributors have moderate power via three-tier system; end consumers have low switching costs but strong brand preferences partially offset this

**4. Supplier Power: Low**
- Hops and malt sourced from many suppliers; commodity inputs with low switching costs

**5. Substitutes: Medium**
- Wine, spirits, hard seltzer, cannabis edibles all compete for the same consumption occasion

**Synthesis:** The governing forces are intense rivalry (fragmentation, slowing growth) and distribution access barriers. Despite strong differentiation, the sheer number of competitors compresses margins. Profit potential is moderate for differentiated brands with distribution relationships; low for undifferentiated entrants.
