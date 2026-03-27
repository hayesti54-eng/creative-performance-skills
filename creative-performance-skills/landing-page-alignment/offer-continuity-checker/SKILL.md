# Offer Continuity Checker

**Category:** landing-page-alignment
**Tier:** pro

## Purpose

This Skill verifies that the offer presented in an ad is exactly reflected on the landing page — same price, same deal terms, same guarantee, same bonus structure, same deadline. Offer discontinuity is the fastest way to destroy trust in a paid campaign. When a visitor clicks an ad for a "$47 limited offer" and lands on a page with $97 pricing and no mention of the deal, the conversion is dead. This Skill catches every version of that before you spend money driving traffic.

---

## When to Use

- You're running a promotional campaign with a specific offer and want to verify continuity before launching
- A landing page has been updated and you need to confirm the offer still matches active ads
- You're running split tests with different offer framings in ads and want to check page alignment for each
- You've had a sudden CVR drop that doesn't match creative performance metrics — offer discontinuity is a common cause
- You're managing multiple offers across multiple campaigns and want to audit all ad-to-page offer alignments at once

---

## Inputs Required

- Ad copy (full text including any offer mentions: price, discount, guarantee, bonus, urgency/scarcity)
- Landing page offer section (pricing, guarantee language, deal terms, bonus presentation)
- The specific offer details as agreed: price, discount amount or percentage, guarantee terms, what's included, deadline
- Any promotion codes referenced in the ad

---

## What This Skill Does

Checks seven offer continuity dimensions between ad and landing page, scores each, identifies discrepancies, flags the conversion risk of each discrepancy, and recommends the specific change needed.

---

## Analysis Workflow

1. **Extract the offer as stated in the ad**
   From the ad copy, extract: stated price or discount, guarantee or risk-reversal language, bonuses mentioned, urgency signals (deadline, limited quantity, limited time), what's included in the offer.

2. **Extract the offer as presented on the landing page**
   From the landing page, extract the same elements: price shown, guarantee language, bonuses shown, urgency signals, what the page says is included.

3. **Check Price Continuity**
   Does the price in the ad match the price on the landing page exactly?
   - Exact match: Clear pass
   - No price in ad + no price on page: Acceptable
   - Price in ad + different price on page: Severe gap
   - No price in ad + price on page: Minor gap (landing page is adding context, which is acceptable)

4. **Check Discount/Deal Continuity**
   If the ad mentions a discount, promo, or deal: does the landing page show the same discount, or has it reverted to full price?

5. **Check Guarantee Continuity**
   If the ad mentions a guarantee (30-day money back, free trial, satisfaction guarantee): does the landing page present the same guarantee prominently, or is it buried or absent?

6. **Check Bonus Continuity**
   If the ad mentions a bonus or freebie included with purchase: is the bonus listed on the landing page?

7. **Check Urgency/Scarcity Continuity**
   If the ad uses time-sensitive language (limited offer, sale ends Sunday, only 50 spots): does the landing page mirror that urgency, or does the page present the offer as evergreen? Urgency-without-confirmation destroys the urgency signal.

8. **Check Inclusion Continuity**
   If the ad describes what's included (X features, Y modules, Z bonuses): does the landing page list the same items?

9. **Check CTA Language Continuity**
   Does the ad CTA ("Start Free Trial," "Claim Your Spot," "Get the Kit") match the landing page CTA button and instruction?

10. **Score and flag**
    For each dimension: Pass / Minor Gap / Severe Gap. Calculate total continuity score. Flag all Severe Gaps for immediate correction before traffic runs.

---

## Output Requirements

**Offer Continuity Scorecard**
| Dimension | Ad Version | Page Version | Score | Risk Level |
| Price | | | | |
| Discount | | | | |
| Guarantee | | | | |
| Bonus | | | | |
| Urgency | | | | |
| Inclusions | | | | |
| CTA | | | | |

**Severe Gap Flags**
Explicit warning for each Severe Gap with the estimated conversion impact and the specific change required to resolve.

**Correction Recommendations**
For each gap: which side to fix (the ad or the page), the specific text or structural change needed.

**Launch Gate Decision**
Should traffic be sent to this page now? Yes (all Pass / Minor Gaps only) / No (one or more Severe Gaps — fix before launching).

---

## Best Practices Applied

- Severe Gaps always require a fix before traffic runs — never launch with known offer discontinuity
- Price discrepancy is the highest-trust-cost gap and must always be corrected
- Urgency signals must be mirrored on the landing page or they are meaningless (and potentially deceptive)
- Minor gaps are acceptable to launch with but should be corrected in the next iteration cycle
- The CTA language continuity check is the easiest fix and should never be missed

---

## Guardrails

- Do not approve a launch with price discrepancy — this is a hard block
- Do not approve a launch where the ad promises a guarantee that the landing page does not mention
- Do not flag different wording as a Severe Gap if the meaning and terms are identical
- Do not assume the landing page is correct — it may be the ad that has an error
- Do not evaluate urgency language continuity in isolation — verify that the urgency claim is accurate to begin with

---

## Example Requests

1. "We're launching a Black Friday campaign tomorrow. Here's the ad copy with our offer details and here's the landing page. Check every offer element and tell me if it's safe to launch."

2. "We had a sudden CVR crash yesterday. No creative changes were made. Can you check if someone accidentally updated the landing page offer details? Here's the current page vs. our active ad."

3. "We're running 3 ads with slightly different offer angles to the same landing page. Check each ad against the page and tell me if any of them have offer discontinuity."
