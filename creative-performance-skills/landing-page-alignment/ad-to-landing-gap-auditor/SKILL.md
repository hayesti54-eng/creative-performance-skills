# Ad-to-Landing Gap Auditor

**Category:** landing-page-alignment
**Tier:** pro

## Purpose

This Skill audits the alignment between an ad and its landing page across five continuity dimensions: promise, offer, emotion, objection handling, and CTA. The gap between what an ad promises and what a landing page delivers is one of the most expensive and least diagnosed problems in paid media. High CTR, low CVR with no obvious creative problem is almost always a landing page continuity failure. This Skill finds it.

---

## When to Use

- CTR is strong but CVR is significantly below benchmark
- You've launched a new ad to an existing landing page and conversions haven't matched expectations
- You want to audit an entire funnel before scaling spend
- A landing page has been updated and you need to check if it still matches the ads pointing to it
- You're running multiple ad concepts to the same landing page and want to know which ones have continuity vs. which are creating a gap
- You're diagnosing poor ROAS on a campaign where creative performance metrics look acceptable

---

## Inputs Required

- Ad copy (full body copy + headline)
- Landing page content (paste text or describe the page structure: headline, subheadline, hero, body, CTA, proof, offer presentation)
- Campaign objective
- Audience awareness stage
- Offer details (price, guarantee, what's included)

---

## What This Skill Does

Audits alignment across five continuity dimensions and scores each one. Produces a gap report identifying specific misalignments, their likely impact on conversion, and the specific fix for each.

---

## Analysis Workflow

1. **Audit Promise Continuity**
   What specific promise does the ad make (explicit or implied)? Does the landing page headline deliver on that exact promise within 3 seconds of arrival? A visitor should land and immediately recognize the match between what the ad said and what the page confirms.
   - Strong match: Landing page headline mirrors ad promise with same language or direct equivalent
   - Partial match: Landing page addresses the topic but with different framing or specificity level
   - Gap: Landing page addresses a different angle than the ad promised

2. **Audit Offer Continuity**
   What offer is presented in the ad (price, discount, bundle, free trial, guarantee)? Does the landing page present the exact same offer, or does the offer change (higher price, different terms, missing discount)? Any offer change between ad and landing page destroys trust and increases bounce intent.

3. **Audit Emotional Continuity**
   What emotional state is the ad activating (excitement, relief, urgency, curiosity, aspiration, skepticism)? Does the landing page maintain that emotional state or shift to a different tone entirely? An ad that activates urgency arriving at a calm educational page breaks the emotional momentum.

4. **Audit Objection Handling Continuity**
   Does the ad address or imply handling any specific objections (price, risk, effort, fit)? If so, does the landing page deepen that objection handling, or does it drop the subject and assume trust has been established?

5. **Audit CTA Continuity**
   What action does the ad CTA request (click to learn more, shop now, get the free X, start your trial)? Does the landing page CTA match in action type, language, and placement? A "Get the Free Guide" ad sending traffic to "Buy Now" creates jarring discontinuity.

6. **Score each dimension**
   For each of the 5 dimensions: Strong Match (no gap), Partial Match (minor gap, not critical), Gap (significant mismatch with conversion impact), Severe Gap (major mismatch likely causing substantial conversion loss).

7. **Calculate the overall continuity score**
   5 Strong Matches = Full continuity (conversion losses are almost certainly not a landing page problem)
   3-4 Strong Matches = Acceptable continuity (minor optimizations available)
   2-3 Gaps = Significant continuity problems (priority fix required)
   4-5 Gaps = Severe continuity failure (do not scale until resolved)

8. **Write the fix specifications**
   For each gap: the specific text, element, or structural change needed on either the ad or the landing page to close the gap.

---

## Output Requirements

**Continuity Audit Table**
| Dimension | Ad Version | Landing Page Version | Score | Gap Description |

**Overall Continuity Score**
Numeric (out of 5) + verbal classification (Full / Acceptable / Significant / Severe)

**Gap Report**
For each gap: dimension, what the ad says, what the page says, the conversion impact, and the specific fix.

**Priority Fix Recommendations**
Ordered by impact: which gaps to close first and exactly what to change.

---

## Best Practices Applied

- Promise continuity is the most critical dimension — the first 3 seconds of page load determines whether the visitor stays
- Offer continuity gaps are the most trust-destroying — any price or terms discrepancy will kill conversion
- Emotional continuity is the most commonly overlooked — operators fix copy mismatches but miss tone mismatches
- CTA continuity is the easiest fix and often the fastest conversion win
- The audit should be run from the perspective of a first-time visitor with the specific ad fresh in their mind

---

## Guardrails

- Do not score continuity by comparing word-for-word matching — concept and emotional alignment matter more than identical language
- Do not recommend fixing the ad when the problem is on the landing page — always specify which side of the gap to close
- Do not declare the landing page problem-free if only 3 of 5 dimensions were auditable — flag incomplete audits
- Do not assume a high CTR means the ad is not contributing to the gap — the ad's promise can create unrealistic expectations that the page can't fulfill
- Do not recommend landing page changes that contradict the brand's primary messaging architecture

---

## Example Requests

1. "Here's our ad copy and our landing page content. Our CTR is 3.8% but CVR is 0.8%. Is there a message gap? Tell me exactly where."

2. "We're running 5 different ads to the same landing page. Audit each ad against the landing page and tell me which ones have continuity and which ones are creating a mismatch."

3. "We just rebuilt our landing page. Before we start sending paid traffic to it, audit it against our top-performing ad to make sure nothing broke."
