# Hypothesis Builder

**Category:** testing
**Tier:** pro

## Purpose

This Skill transforms a vague creative idea or hunch into a structured, testable hypothesis that can drive a real A/B test. It forces documentation of the variable being tested, the rationale behind the test, the expected outcome, and the success metric — before a single dollar is spent. Teams that skip hypothesis documentation run tests they can't learn from. This Skill makes that mistake impossible.

---

## When to Use

- You have an idea for a new creative direction and want to turn it into a proper test
- You've spotted something in performance data and want to investigate it with a controlled test
- You're planning a testing roadmap and need documented hypotheses for each planned test
- A stakeholder wants to know why you're running a specific test
- You want to validate whether a past test was run correctly (did it have a proper hypothesis?)
- You're onboarding a creative or media buyer and need to teach hypothesis-first testing

---

## Inputs Required

- The creative idea or hunch you want to test (describe it plainly)
- The specific metric you want to improve (CTR, CVR, ROAS, hook rate, CPL, etc.)
- Current benchmark for that metric (what does it need to beat?)
- The control creative or current baseline being tested against
- Any past data or insight that inspired this test (optional but strengthens the hypothesis)
- Audience and campaign context

---

## What This Skill Does

Structures a creative hypothesis into a standardized five-part format: the belief statement, the variable being changed, the rationale, the expected outcome, and the success metric. Evaluates whether the hypothesis is testable, falsifiable, and properly isolated before flagging it as test-ready.

---

## Analysis Workflow

1. **Extract the core belief**
   What do you actually believe will happen if you make this change? State it plainly. "I believe that leading the hook with a specific outcome number will increase CTR compared to our current problem-led hook."

2. **Isolate the single variable**
   Identify exactly one element being changed. If more than one element is changing, the test is confounded. Flag and force isolation: "You are changing the hook AND the visual. These must be split into two separate tests."

3. **Write the rationale**
   Why do you believe this variable matters? Anchor the rationale in one of: (a) performance data from this account, (b) customer language from reviews or calls, (c) a winning pattern from a past test, or (d) a testable principle of direct response. Rationale based on "I have a feeling" is flagged as weak.

4. **Define the control and variant**
   Control: [exact description of what is NOT changing]. Variant: [exact description of the one thing that IS changing]. These must be explicit and unambiguous.

5. **Write the success metric and threshold**
   Define: what specific metric must improve, by how much, to call this test a winner. "If CTR increases by more than 20% above the control at $200+ spend, the variant wins." Avoid open-ended success criteria.

6. **Set the minimum valid spend threshold**
   Based on campaign objective, CPC, and conversion rate, estimate the minimum spend required to reach meaningful signal. If budget is below this threshold, flag the test as likely inconclusive and adjust the success threshold accordingly.

7. **Evaluate hypothesis quality**
   Score the hypothesis: Testable (yes/no), Falsifiable (yes/no), Variable isolated (yes/no), Rationale strength (strong / directional / weak). Output a test-readiness rating.

8. **Write the final formatted hypothesis**
   Output in the standard format documented in Output Requirements.

---

## Output Requirements

**Structured Hypothesis Document**
```
HYPOTHESIS: [One sentence — "I believe that [X change] will [improve Y metric] because [Z rationale]"]
VARIABLE: [The single element being changed]
CONTROL: [Exact description of control]
VARIANT: [Exact description of variant]
RATIONALE: [What data, customer language, or principle supports this test]
SUCCESS METRIC: [Specific metric + threshold + minimum spend for validity]
EXPECTED OUTCOME: [What you expect to happen and by approximately how much]
TEST-READINESS: [READY / NEEDS REFINEMENT + specific issues to resolve]
```

**Quality Flags** (if applicable)
Any issues that would make this test inconclusive: multiple variables changing, insufficient budget, wrong metric for the objective, audience too small, control too different from variant.

---

## Best Practices Applied

- One variable per test — this is the non-negotiable rule of valid A/B testing
- Rationale must be anchored in real evidence, not intuition
- Success metrics are pre-defined, not decided after results come in
- Minimum spend thresholds prevent reading too much into underspent tests
- Falsifiability is required — a hypothesis that can't be disproven is not testable

---

## Guardrails

- Do not accept vague hypotheses like "let's see if a better creative performs better" — force specificity
- Do not build a hypothesis around two changing variables — always flag and split
- Do not set success metrics after the fact — they must be written before the test runs
- Do not approve a hypothesis without an explicit control described
- Do not accept "industry best practice" as rationale without account-specific anchoring

---

## Example Requests

1. "I think our hooks are too long. I want to test a 5-word hook vs our current 15-word hook. Help me build a proper hypothesis for this test."

2. "We've seen a lot of customers mention 'fast results' in reviews. I want to test leading with speed as a hook. Write the hypothesis for me."

3. "I have 6 creative ideas I want to test this quarter. Turn each one into a proper hypothesis document with success metrics."
