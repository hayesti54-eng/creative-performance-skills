# Concept Performance Reporter

**Category:** reporting
**Tier:** pro

## Purpose

This Skill generates performance reports at the concept level — not the individual ad level, but the angle, format, and messaging approach level. When you're running 15 ads, what you need to know is not which specific ad won, but which concept won. "The founder story angle with a specific outcome hook outperformed the listicle format across all 6 variations we tested." That is concept-level intelligence, and it is how creative programs get smarter faster.

---

## When to Use

- You've run multiple ads with the same underlying concept and want to evaluate the concept as a whole
- You want to compare which formats, angles, or messaging approaches are winning at a category level
- You're building a creative learning log and want to track concept-level performance trends
- You want to brief new creative from concept-level insights, not individual ad results
- You've run a batch test across multiple hooks and want to evaluate hook category performance

---

## Inputs Required

- Performance data for a set of ads
- Creative groupings: which ads belong to the same underlying concept, angle, or format category
- Campaign objective and primary metric
- Date range
- Benchmarks
- Concept labels (e.g., "Founder Story," "Before-After," "Testimonial Block," "Listicle Format")

---

## What This Skill Does

Groups individual ad performance data by concept category, calculates concept-level aggregate metrics, ranks concepts by performance, identifies which concept category is winning and which is losing, and generates concept-level briefing implications for the next creative round.

---

## Analysis Workflow

1. **Group ads by concept category**
   Organize all ads into their underlying concept, format, or angle groups. Example: all 4 testimonial ads together, all 3 founder story ads together, all listicle ads together.

2. **Calculate concept-level aggregate metrics**
   For each concept group: average CTR, average CVR/ROAS, total spend, average CPM, average frequency. If video: average hook rate and hold rate.

3. **Rank concept categories by primary metric**
   Sort concept groups by whatever metric matters most for the campaign objective. Flag which categories beat benchmark vs. missed.

4. **Identify the winning concept category**
   Which format/angle category is performing best? Note the margin of difference from the next best. Is the win consistent across all ads in the category, or driven by one outlier?

5. **Identify the losing concept category**
   Which format/angle category is consistently underperforming? Flag whether this is a kill-category (no concept in this category has worked) or a fix-category (some ads in this category showed signal but the execution wasn't right).

6. **Identify concept-level anomalies**
   Are there outlier ads that are over- or underperforming their concept category average? These anomalies contain the most information — they isolate what variables beyond the concept category are driving performance.

7. **Write the concept performance brief**
   Translate concept-level data into creative direction for the next round: "Testimonial concepts are outperforming all other formats by 40% on CVR. Priority for next period: brief 4 new testimonial concepts. Founder story concepts are underperforming — the angle is not landing for this audience at this awareness stage. Deprioritize until we have a strong retargeting audience to test them with."

---

## Output Requirements

**Concept Performance Summary Table**
| Concept Category | Ads in Group | Avg CTR | Avg CVR | Avg ROAS | vs Benchmark | Verdict |

**Concept Rankings**
Ranked 1 through N by primary metric. Winning concept category at the top.

**Anomaly Analysis**
Outlier ads flagged with explanation of what they might reveal about variables beyond concept category.

**Next Round Creative Brief Implications**
For each concept category: more of this / less of this / fix this / kill this — with one-line rationale.

---

## Best Practices Applied

- Concept-level analysis reveals patterns that individual ad analysis misses
- Consistency within a concept category is more important than a single outlier performance
- Anomalies in the data (ads that break category trends) are the most valuable signal for variable isolation
- Next round implications must flow directly from the data — not from creative preference
- Category verdicts should be validated across at least 3 ads before declaring a category pattern

---

## Guardrails

- Do not evaluate a concept category on fewer than 2 ads — single ad data does not represent a concept
- Do not declare a concept category "dead" from one test round — direction is confirmed over multiple rounds
- Do not aggregate concept performance across completely different audiences — audience differences contaminate concept-level conclusions
- Do not confuse a bad execution (poor creative quality) with a bad concept — quality must be evaluated alongside performance
- Do not ignore budget allocation differences between concept groups — an underfunded category may underperform due to spend, not concept quality

---

## Example Requests

1. "We ran 12 ads last month — 4 testimonial concepts, 4 founder story concepts, and 4 listicle concepts. Analyze them by concept category and tell me which categories to invest in next month."

2. "I've been running UGC and polished studio creative in parallel for 6 weeks. Compare their performance at the concept level — not just individual ads — and tell me what the data says."

3. "We tested 6 different hook angles last month across the same ad body copy. Analyze the hook angle categories and tell me which approach is winning."
