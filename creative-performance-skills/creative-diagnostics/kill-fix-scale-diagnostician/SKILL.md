# Kill / Fix / Scale Diagnostician

**Category:** creative-diagnostics
**Tier:** pro

## Purpose

This Skill analyzes performance creative and assigns a structured Kill, Fix, or Scale decision to each asset based on real metrics, behavioral signals, and creative factors — not gut feel. It eliminates the most expensive creative mistake in paid social: scaling bad ads and killing good ones. Every decision is tied to evidence, and every Fix recommendation includes specific changes to test.

---

## When to Use

- You have a set of active or recently paused ads and need to decide what to do with each one
- You're doing a weekly or monthly creative review and need structured output
- An ad is underperforming but you're not sure if it's the creative or the targeting
- You have a top-performing ad and want to understand what's driving the win before scaling
- You're presenting creative decisions to a client or stakeholder and need defensible reasoning
- You've run a test and need to classify results into actionable next steps

---

## Inputs Required

- Ad creative performance data (minimum: spend, CTR, CPC, ROAS or CVR, frequency, CPM)
- Creative descriptions or copies of the ads (headline, body copy, visual description or screenshot)
- Benchmark metrics (account average or industry average for CTR, CPC, ROAS)
- Campaign objective (awareness, traffic, conversions, leads)
- Date range of data
- Optional: hook rate (3-second video views / impressions), hold rate (ThruPlay / 3-sec views), outbound CTR

---

## What This Skill Does

Runs each creative through a five-layer diagnostic framework (distribution health, hook performance, engagement quality, conversion signal, and creative fatigue index) to assign one of three classifications — Kill, Fix, or Scale — with specific rationale and next action for each.

---

## Analysis Workflow

1. **Establish benchmarks**
   Define account-level or category-level baseline for CTR, CPC, ROAS/CVR, CPM, and frequency. If not provided, use standard Meta performance benchmarks by vertical.

2. **Run distribution health check**
   Evaluate CPM relative to benchmark. High CPM = delivery problem (audience exhaustion, low relevance score, competitive pressure). Flag ads where CPM is >40% above benchmark.

3. **Run hook performance analysis**
   If video: hook rate <25% is a weak hook signal. Hook rate >40% is a strong hook signal. If static: evaluate opening line of copy for specificity, urgency, and relevance. Flag weak hooks for Fix queue.

4. **Run engagement quality check**
   CTR (all) vs. CTR (outbound/link). Large gap = the creative is generating curiosity clicks but not intent clicks. Evaluate if this is a headline/visual mismatch or offer mismatch.

5. **Run conversion signal analysis**
   Compare CVR or ROAS to benchmark. Low CTR + low CVR = creative problem at both stages. High CTR + low CVR = landing page problem (flag for landing page audit, not creative kill). Low CTR + high CVR = audience is wrong, not creative.

6. **Run fatigue index**
   Frequency >3.5 in a 7-day window = fatigue risk. Frequency >6 in 30-day window = active fatigue. If performance has declined >25% MoM and frequency is elevated, classify as Kill or Fix.

7. **Assign Kill / Fix / Scale classification**
   - **Kill:** CPM elevated AND CTR below benchmark AND CVR below benchmark AND frequency >4 AND no improvement path evident
   - **Fix:** One or two layers failing but core offer or angle shows signal. Specify exactly what to fix: hook, headline, CTA, proof element, or visual
   - **Scale:** CTR above benchmark AND CVR above benchmark AND frequency below fatigue threshold AND ROAS/CVR target met or exceeded

8. **Write Fix recommendations**
   For every Fix classification, output exactly what to change. Be specific: "Rewrite opening hook to lead with the outcome, not the product." Not: "Improve the hook."

9. **Output structured decision table**
   Produce a clean table: Creative ID or Name | Classification | Primary Signal | Fix Recommendation or Scale Action | Priority

---

## Output Requirements

**Kill/Fix/Scale Decision Table**
| Creative | Classification | Primary Evidence | Action | Priority |
One row per creative asset. No fluff.

**Diagnostic Summary**
- How many Kills, Fixes, Scales
- The most common failure pattern across the set
- Top recommended next test based on winners

**Fix Specifications**
For each Fix: the specific layer failing, the specific change required, and the expected impact metric.

**Scale Specifications**
For each Scale: what's working, recommended budget increase range (conservative: 20-30%; aggressive: 50%+), and whether to duplicate or expand targeting.

---

## Best Practices Applied

- Decisions are multi-signal, not single-metric — one bad metric does not equal a Kill
- High CTR + low CVR is diagnosed as a landing page problem, not a creative kill
- Fatigue is always evaluated alongside performance trend, not frequency alone
- Fix recommendations are specific and testable, not directional platitudes
- Scale recommendations include a magnitude (20%, 50%, duplicate) not just "scale this"
- Every classification has a written rationale traceable to data

---

## Guardrails

- Do not recommend Kill based on spend alone — underspent ads are not diagnosable
- Do not recommend Scale before spend has reached statistical significance (minimum $50-100 per ad for most campaigns)
- Do not classify an ad as failing without checking if the campaign objective matches the metric being evaluated
- Do not confuse audience exhaustion with creative failure — always check CPM trend
- Do not assume all low-CTR ads are creative failures — audience mismatch produces identical symptoms
- Do not make Fix recommendations that change multiple variables — each fix must isolate one variable

---

## Example Requests

1. "Here are 8 ads from our last 30 days with their metrics. Tell me which ones to kill, which to fix, and which to scale — and exactly what to do with each."

2. "Our top ad from last month had a 4.2% CTR but our ROAS dropped in week 3. Is this fatigue or something else? What should I do with it?"

3. "We have 12 active ads in our account. Here's the data. Run a full Kill/Fix/Scale analysis and give me a prioritized action list for this week."
