# Creative Fatigue Pattern Reviewer

**Category:** creative-diagnostics
**Tier:** pro

## Purpose

This Skill identifies creative fatigue before it destroys campaign performance. It goes beyond checking frequency — it reads the behavioral signature of a fatiguing creative across multiple metric dimensions and tells you exactly when the creative started dying, why it's dying, and what type of fatigue it is. Different fatigue patterns require different responses, and this Skill distinguishes between them so you don't make the wrong call.

---

## When to Use

- Performance on an ad has declined over time but frequency looks normal
- You're seeing rising CPM without audience size changes
- CTR is holding but CVR is dropping — a subtle fatigue signal most teams miss
- You want to set proactive fatigue thresholds before an ad starts declining
- You're managing a winning ad and want to know when to rotate
- You want to understand which creative types in your account fatigue fastest

---

## Inputs Required

- Time-series performance data: minimum 4 weeks of weekly breakdowns (CTR, CPC, CVR or ROAS, CPM, frequency, impressions, spend)
- Creative type (video, static, carousel, UGC, founder story, etc.)
- Audience size estimate or targeting setup description
- Campaign budget (daily or lifetime) and delivery method (standard or accelerated)
- Optional: hook rate and hold rate trend over time for video assets

---

## What This Skill Does

Reads multi-metric time-series performance to detect fatigue signatures, classify the fatigue pattern type, identify when the decline inflection point occurred, and produce a specific rotation or refresh recommendation based on the pattern.

---

## Analysis Workflow

1. **Map performance trend by week**
   Build a mental week-by-week trend for each key metric: CTR, CVR/ROAS, CPM, frequency, CPC. Identify direction (improving, flat, declining) and rate of change.

2. **Identify the inflection point**
   Find the specific week where performance peaked or where decline began. Note what changed in that window (frequency threshold crossed, audience size reached, creative type, day of week patterns).

3. **Classify the fatigue pattern**
   Match the metric signature to one of five fatigue pattern types:

   - **Pattern A — Hook Fatigue:** CTR declining, hold rate and CVR still acceptable. The opening is worn out but the offer still works. Fix: new hook, same body copy.
   - **Pattern B — Offer Fatigue:** CTR holding but CVR collapsing. Audience has seen the offer too many times and stopped believing it or caring. Fix: new proof, new guarantee framing, new CTA.
   - **Pattern C — Format Fatigue:** All metrics declining uniformly. The creative type itself is worn out in this audience. Fix: switch format (static to video, UGC to polished, etc.).
   - **Pattern D — Audience Exhaustion:** CPM rising rapidly alongside frequency, CTR flat or declining. The available audience pool is saturated. Fix: expand targeting, use lookalike, or pause and reset.
   - **Pattern E — Seasonal or External Fatigue:** Decline aligns with external date event (holiday, news event, seasonal shift). Not a creative failure. Fix: update angle to current context.

4. **Check frequency against fatigue threshold**
   Soft threshold: frequency 3.0-3.9 in 7 days = monitor closely. Hard threshold: frequency 4.0+ in 7 days = active fatigue risk. Lifetime frequency >8 in 30 days = likely exhausted for this creative.

5. **Measure performance decay rate**
   Calculate week-over-week % change in CTR and CVR. Decay rate >15% WoW = aggressive fatigue. Decay rate 5-15% WoW = moderate fatigue. Decay rate <5% = acceptable aging.

6. **Estimate remaining useful life**
   Based on decay rate and current performance gap to benchmark, estimate how many additional weeks before this creative crosses kill threshold. Express as a range: "1-2 weeks before kill threshold at current decay rate."

7. **Write rotation recommendation**
   Specify: (a) whether to pause immediately or run until threshold, (b) exactly what type of replacement to test first based on the fatigue pattern, (c) whether to refresh the existing creative or replace entirely.

---

## Output Requirements

**Fatigue Diagnostic Report**
- Creative name/ID
- Fatigue Pattern Classification (A through E with label)
- Inflection point (week)
- Current performance vs. benchmark
- Remaining useful life estimate
- Decay rate (CTR and CVR WoW %)
- Frequency status

**Rotation Recommendation**
- Pause now or continue with timeline
- Recommended refresh type or replacement format
- Variable to change first (hook, offer, format, audience)

**Fatigue Calendar**
If multiple creatives analyzed: a priority table showing which assets need rotation in Week 1, Week 2, Week 3+ based on decay rate and remaining life.

---

## Best Practices Applied

- Fatigue is multi-dimensional — frequency alone is not fatigue
- Hook fatigue and offer fatigue require different fixes
- Audience exhaustion is not creative failure — the diagnosis changes the action
- Proactive rotation before kill threshold preserves performance momentum
- Fatigue patterns differ by creative type (video fatigues faster than static in high-frequency accounts)
- Time-series data always outranks single-point snapshot data for fatigue diagnosis

---

## Guardrails

- Do not declare fatigue from a single week of declining metrics — check for external causes first (budget changes, audience changes, bid strategy changes)
- Do not recommend rotating a creative that is still above benchmark, regardless of frequency
- Do not diagnose fatigue from CPM alone — rising CPM can be seasonal or competitive, not creative-driven
- Do not recommend the same creative type as replacement when Format Fatigue is detected
- Do not conflate low volume ads (under $50 spend) with fatigued ads — insufficient data

---

## Example Requests

1. "Here's 6 weeks of weekly data on our top 3 ads. One of them has been declining since week 3 but frequency is only 2.8. What's happening and what should I do?"

2. "Our video ad had a great first two weeks and now everything is dropping. Hook rate is still 38% but our CVR fell from 3.2% to 1.1%. Is this fatigue? What kind?"

3. "We have 5 active ads and I want to know which ones to plan rotation for in the next 3 weeks. Here's the data. Build me a fatigue calendar."
