# Message Match Reviewer

**Category:** landing-page-alignment
**Tier:** pro

## Purpose

This Skill evaluates the specific language and messaging match between an ad and its destination page — going deeper than structural continuity to analyze whether the exact words, claims, tone, and framing used in the ad are reflected, confirmed, and extended on the landing page. Message match is the principle that the language a visitor was responding to when they clicked should be reinforced immediately upon arrival. When it is, trust builds. When it is not, trust erodes.

---

## When to Use

- You want to check whether your landing page headline mirrors the most compelling language from your ad
- You're running multiple audiences and ads with different messaging and want to verify each message is matched on the page
- Your landing page performs differently for different traffic sources and you want to identify which message is creating the mismatch
- You're building dynamic landing pages (or considering it) and want to know which message to match
- You want to audit ad campaigns after landing page copy changes

---

## Inputs Required

- Ad copy (headline, primary text, and any on-image/video text)
- Landing page copy (headline, subheadline, hero section, and above-the-fold content minimum)
- The specific audience and their awareness stage
- The primary claim or hook driving the ad's CTR

---

## What This Skill Does

Evaluates the message match between the ad's most compelling language and the landing page's first-impression content. Identifies specific language the visitor was responding to and verifies whether that exact language or its equivalent is confirmed on the page within the first scroll.

---

## Analysis Workflow

1. **Extract the ad's primary message hook**
   What is the single most compelling thing the ad communicates? The hook that drove the click? Isolate the specific claim, emotion, or promise that is most likely the reason the visitor clicked.

2. **Evaluate the landing page headline match**
   Does the landing page headline directly or closely mirror the ad's primary hook? Test: if the visitor saw the landing page headline first, would they recognize it as the "more of what I was promised"?
   - Direct match: Same claim in same language
   - Conceptual match: Same idea with different (but equivalent) words
   - Tangential match: Related topic but different claim or different specificity
   - No match: Different angle entirely

3. **Evaluate the subheadline and hero text match**
   Does the subheadline or hero paragraph extend and deepen the ad's primary message, or does it pivot to a different topic?

4. **Evaluate specificity match**
   If the ad used a specific number, claim, or outcome ("lose 18 lbs in 6 weeks"), does the landing page immediately confirm that specific claim, or does it speak in vague generalities? Specificity downgrades (ad: specific, page: vague) destroy the credibility built by the specific ad claim.

5. **Evaluate tone and voice match**
   Is the language register of the ad (urgent, conversational, authoritative, empathetic, playful) matched by the landing page? A casual, peer-to-peer UGC ad driving to a formal corporate landing page creates jarring discontinuity.

6. **Score message match**
   Rate the overall message match on a 4-point scale:
   - Strong: Headline, subheadline, tone, and specificity all aligned — visitor sees continuity immediately
   - Good: Headline and concept aligned, minor tone or specificity differences
   - Weak: Conceptually related but materially different language, claim, or specificity level
   - Broken: Different angle entirely — visitor must re-orient on arrival

7. **Write the message match recommendations**
   Specific landing page copy changes (headline rewrites, subheadline edits, or hero text additions) that would close the match gap.

---

## Output Requirements

**Message Match Analysis**
- Primary hook extracted from ad
- Landing page headline as written
- Match score: Strong / Good / Weak / Broken
- Gap description (specific language or framing divergences)

**Specificity Match Check**
- Specific claims in ad vs. landing page — confirmed / downgraded / missing

**Tone Match Check**
- Ad tone description vs. landing page tone description — aligned / divergent

**Recommended Headline Rewrites**
2-3 alternative landing page headlines that would create Strong message match with this specific ad.

---

## Best Practices Applied

- The landing page headline is the most important single element of message match — it is the first thing the visitor reads
- Specificity match is critical — a specific ad driving to vague page language signals that the claim was false or inflated
- Tone match is invisible when correct and viscerally wrong when broken
- Message match is audience-specific — the same landing page may have strong match for one ad and weak match for another
- Dynamic headline testing is the most direct solution to multi-ad message match problems

---

## Guardrails

- Do not recommend making the landing page headline identical to the ad if it would harm the page's standalone performance
- Do not score message match as Broken based on wording differences alone — evaluate whether the concept and claim are aligned
- Do not recommend match improvements that would create compliance or legal issues
- Do not assume the ad headline is the primary hook — sometimes the visual or first line of body copy is what drove the click
- Do not evaluate message match from a desktop perspective only when the primary traffic source is mobile

---

## Example Requests

1. "Our ad says 'Stop wasting 3 hours a week on manual reporting' and our landing page says 'The all-in-one analytics platform.' Is that a message match problem?"

2. "We have 4 different ads running to the same landing page. Check the message match for each ad and tell me which ones are well-matched and which need a different destination."

3. "Rewrite our landing page headline so it creates strong message match with our top-performing ad. Here's the ad and here's the current headline."
