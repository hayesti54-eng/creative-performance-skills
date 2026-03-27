# Creative Report Generator

**Category:** reporting
**Tier:** pro

## Purpose

This Skill generates structured, decision-oriented creative performance reports from raw ad data. A creative report has one purpose: equip the reader to make better creative decisions faster. This Skill eliminates the two failure modes of most creative reports — too long with too many charts and no clear decisions, or too short with only vanity metrics and no actual analysis. Every report this Skill generates is built around actions, not aesthetics.

---

## When to Use

- You need a weekly or monthly creative performance report for your team or a client
- You've completed a test round and need to summarize the results
- You want to present creative performance data to a stakeholder who doesn't live in the ads manager
- You're doing a quarterly review of your creative program and need a structured summary
- You want to build a recurring reporting template that can be updated weekly

---

## Inputs Required

- Performance data: spend, impressions, CTR, CPC, CPM, CVR or ROAS, frequency, reach
- Creative descriptions or IDs for each asset reported
- Date range
- Previous period's data (for comparison) — optional but strongly recommended
- Account benchmarks or goals
- Campaign objectives
- Optional: hook rate and hold rate for video assets

---

## What This Skill Does

Generates a structured creative performance report organized into: executive summary, Kill/Fix/Scale decisions, winner analysis, loser analysis, format performance summary, next period recommendations, and appendix data. The report is scannable in under 3 minutes and every section points to a decision or action.

---

## Analysis Workflow

1. **Run Kill/Fix/Scale classification**
   Before writing the report, classify every creative as Kill, Fix, or Scale using the diagnostic criteria from the Kill/Fix/Scale Skill. These classifications drive the entire report structure.

2. **Calculate performance vs. benchmark**
   For each metric: this period vs. last period vs. account benchmark. Flag anything more than 20% above or below benchmark.

3. **Identify the top 3 performers and bottom 3 performers**
   Top performers: what's working and why. Bottom performers: primary failure mode for each.

4. **Identify format-level patterns**
   Aggregate performance by creative type (video vs. static, UGC vs. polished, short-form vs. long-form). Are there format-level trends beyond individual creative performance?

5. **Identify the primary learning from this period**
   What single most important thing did the data teach us this period? State it in one sentence.

6. **Write next period recommendations**
   Based on the data: what specific creative decisions should be made next period? These must be concrete: "Kill ad IDs 3, 7. Fix ad IDs 1, 4 (change hook). Scale ad ID 6 with 40% budget increase. Brief 2 new concepts testing the objection angle."

7. **Structure the report**
   Organize in the exact output format below. Every section is required. Nothing is padded.

---

## Output Requirements

**Creative Performance Report**

```
CREATIVE PERFORMANCE REPORT
Period: [Date Range]
Prepared by: [Name or Claude Code]

EXECUTIVE SUMMARY (3 sentences max)
[What period this covers. Top-line performance vs. benchmark. The #1 decision driven by this data.]

PERFORMANCE DASHBOARD
| Metric        | This Period | Last Period | Benchmark | Status |
| Spend         |             |             |           | ✓/⚠/✗ |
| Impressions   |             |             |           |        |
| CTR           |             |             |           |        |
| CPC           |             |             |           |        |
| CPM           |             |             |           |        |
| CVR / ROAS    |             |             |           |        |
| Avg Frequency |             |             |           |        |

KILL / FIX / SCALE DECISIONS
Kill: [ID/Name] — [one-line reason]
Fix: [ID/Name] — [specific change required]
Scale: [ID/Name] — [recommended action + magnitude]

TOP PERFORMERS
1. [Creative] — [What worked + key metric]
2. [Creative] — [What worked + key metric]
3. [Creative] — [What worked + key metric]

UNDERPERFORMERS
1. [Creative] — [Primary failure mode]
2. [Creative] — [Primary failure mode]
3. [Creative] — [Primary failure mode]

FORMAT PERFORMANCE SUMMARY
[2-3 sentences on which creative formats are performing above or below average this period]

PRIMARY LEARNING THIS PERIOD
[Single most important insight from the data — one sentence, specific, actionable]

NEXT PERIOD RECOMMENDATIONS
1. [Specific action]
2. [Specific action]
3. [Specific action]

APPENDIX: Full Creative Data Table
[Raw data table if needed]
```

---

## Best Practices Applied

- Executive summary is 3 sentences maximum — if it requires more, it's not a summary
- Every section points to a decision — no section exists just to show data
- Kill/Fix/Scale decisions are stated explicitly, not implied
- Format-level patterns are surfaced — individual creative data without format-level context misses the bigger trend
- The primary learning is single, specific, and stated in one sentence — broad multi-point learnings are not actionable

---

## Guardrails

- Do not report vanity metrics (likes, shares, reach) as primary performance indicators unless that is the campaign objective
- Do not make the report longer than it needs to be — every additional paragraph reduces the chance it gets read
- Do not include data without a decision implication — if a data point doesn't drive a decision, it doesn't belong in the report
- Do not hedge every conclusion — state Kill/Fix/Scale decisions with confidence
- Do not report without comparison data — single-period snapshots without context are uninterpretable

---

## Example Requests

1. "Here's our Meta ads data for the last 30 days across 8 creatives. Generate a complete creative performance report I can send to the client."

2. "Build me a weekly creative report template I can fill in each Monday with that week's data and send to the team in under 5 minutes."

3. "We just finished a 4-week test round. Here's all the data. Write a performance report that summarizes what we learned and exactly what we're doing next period."
