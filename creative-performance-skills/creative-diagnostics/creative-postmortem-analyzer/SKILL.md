# Creative Postmortem Analyzer

**Category:** creative-diagnostics
**Tier:** pro

## Purpose

This Skill runs a structured postmortem on a completed creative test or a paused/killed ad to extract learnable intelligence from the result. The purpose is not to relitigate the decision — it's to build an institutional knowledge base from every test so the next creative is better than the last. Without postmortems, teams repeat the same mistakes. With them, every dead ad contributes to the system.

---

## When to Use

- A test has completed and you need to document what was learned
- A creative was killed and you want to understand the specific failure mode
- A creative massively outperformed expectations and you want to understand why
- You're doing a quarterly creative review and need to synthesize learnings across the test history
- You're onboarding a new creative to the account and want them to understand what has already been learned
- You're building a "what works" creative document for this brand or account

---

## Inputs Required

- Creative description (copy, headline, visual direction or screenshot)
- Creative type / format (video, static, carousel, etc.)
- Performance results (CTR, CVR, ROAS, spend, impressions, frequency at pause)
- Test hypothesis (if documented) or stated reason for making this creative
- Benchmark for this account/campaign
- Audience targeted
- Date range active
- Outcome classification (winner, loser, inconclusive)
- Optional: competing creatives tested against this one

---

## What This Skill Does

Runs a structured five-part postmortem: hypothesis evaluation, performance attribution, failure or success mode classification, insight extraction, and knowledge documentation. Outputs a postmortem report that is file-able into a creative learning log.

---

## Analysis Workflow

1. **Reconstruct the hypothesis**
   If a hypothesis was documented, evaluate whether the test was valid (proper variable isolation, sufficient spend, correct audience). If no hypothesis was documented, reconstruct what was implicitly being tested based on the creative direction.

2. **Classify the outcome type**
   Outcomes are not binary win/lose. Classify as one of five types:
   - **Clear Winner:** Beat benchmark on primary metric with statistical confidence
   - **Directional Winner:** Outperformed but insufficient spend for confidence — warrants retest
   - **Flat:** No meaningful difference from benchmark or control — neither proves nor disproves hypothesis
   - **Directional Loser:** Underperformed but pattern suggests a fixable variable
   - **Clear Loser:** Significantly underperformed with clear failure signal

3. **Identify the failure mode or success driver**
   For losers: which element failed? Isolate to one of: hook, headline, offer, visual, audience mismatch, landing page disconnect, format mismatch, or wrong awareness stage. For winners: which element led the win? Document specifically.

4. **Extract the primary learning**
   State the learning as a testable, generalizable rule: "For this audience, hooks leading with the outcome outperform hooks leading with the problem." Be specific to this account context — not generic marketing advice.

5. **Extract the secondary learning**
   Document any unexpected signal — something the data showed that wasn't being tested for but is worth noting.

6. **Write the "Next Test" recommendation**
   Based on the postmortem, what is the most logical next creative test? What hypothesis does it test? What variable does it isolate?

7. **Write the knowledge log entry**
   Format as a single, file-able insight entry: Date | Creative Description | Outcome | Primary Learning | Next Test Recommended

---

## Output Requirements

**Postmortem Report**
- Creative ID / name
- Outcome classification
- Hypothesis evaluation (was the test valid? what was actually being tested?)
- Failure mode or success driver
- Primary learning (specific and actionable)
- Secondary learning (unexpected signal)
- Next test recommendation with hypothesis

**Knowledge Log Entry**
One-line format ready to paste into a creative learning log:
`[Date] | [Creative] | [Outcome] | [Learning] | [Next Test]`

**Pattern Flag** (if applicable)
If this outcome matches a pattern seen in previous tests, flag it: "This is the third time a problem-led hook underperformed for this audience — this is now a confirmed pattern, not a one-off."

---

## Best Practices Applied

- Postmortems are run on both winners and losers — you learn as much from what works as from what fails
- Learning extraction is specific, not generic — "the hook failed" is not a learning; "the hook failed because it led with the product name instead of the outcome" is a learning
- Next test recommendations are derived from the postmortem, not invented independently
- Flat outcomes are documented as "hypothesis unresolved" and scheduled for retest
- Pattern recognition across multiple postmortems is more valuable than individual postmortems

---

## Guardrails

- Do not attribute failure to one variable when multiple variables changed between tests — flag as confounded test
- Do not declare a winner from underspent tests — classify as directional and retest
- Do not write generic learnings ("improve the hook") — every learning must be specific to the test and account context
- Do not assume the creative failed if the landing page was the likely failure point
- Do not skip documenting inconclusive tests — "no signal" is still intelligence

---

## Example Requests

1. "Our founder story video ran for 3 weeks, spent $800, CTR was 1.4% vs our 2.1% benchmark, and we paused it. Run a postmortem and tell me what we actually learned."

2. "We had a surprise winner last month — a listicle static that beat our best video by 40% on ROAS. I want to understand exactly why it won and what we should test next."

3. "I want to build a creative learning log from our last 8 test postmortems. Here's the data for each one. Give me the full postmortems and the log entries."
