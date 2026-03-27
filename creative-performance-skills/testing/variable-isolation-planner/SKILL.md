# Variable Isolation Planner

**Category:** testing
**Tier:** pro

## Purpose

This Skill takes a creative idea that involves multiple changing elements and breaks it into a properly sequenced series of isolated single-variable tests. It is the enforcer of the most important rule in creative testing: one variable per test. Without variable isolation, you cannot determine what drove the result. This Skill prevents teams from running tests they can't learn from.

---

## When to Use

- You want to test a new creative direction but it involves changing multiple things at once
- A creative "refresh" has changed the hook, headline, visual, and offer simultaneously
- You're comparing two completely different ads and want meaningful learnings from the comparison
- You've run a test and the results are ambiguous — this Skill helps diagnose whether confounding was the cause
- You want to build a logical sequence for iterating on an existing winner
- A team member has proposed testing "a whole new creative" and you need to structure the learning properly

---

## Inputs Required

- Description of the creative change or new creative concept you want to test
- Description of the current control creative (what it contains: hook, headline, offer, visual, CTA, format)
- The primary metric you're trying to improve
- Available budget and testing timeline
- Optional: which element you most believe is the problem or opportunity

---

## What This Skill Does

Audits a proposed creative change for variable isolation violations, identifies all variables that are changing simultaneously, and restructures the change into a sequenced series of single-variable tests with a logical order that builds toward the full creative iteration efficiently.

---

## Analysis Workflow

1. **Inventory the proposed change**
   List every element that is different between the control and the proposed variant. Elements to check: hook (opening line/image), headline, body copy structure, proof element, offer framing, CTA text, CTA placement, visual style, format, length, talent, color/design.

2. **Count simultaneous variable changes**
   If 0-1 elements are changing: test is properly isolated. Proceed.
   If 2-3 elements are changing: restructure into sequential tests.
   If 4+ elements are changing: this is a new creative, not a test iteration. Flag this explicitly and help the user decide whether to run it as a proof-of-concept or isolate it.

3. **Identify the highest-impact variable**
   Of all the changing elements, which one is most likely to drive the metric the user cares about? This test runs first. Rationale: test the highest-leverage variable first so if it wins, you know what moved the needle.

4. **Build the isolation sequence**
   Create a test order: Test 1 (highest-impact variable) → Test 2 (second variable, building on Test 1 results) → Test 3 (third variable, incorporating results from Tests 1 and 2). Each test must use the winner of the prior test as its control.

5. **Write control and variant descriptions for each test**
   For Test 1: Control = existing ad unchanged. Variant = existing ad with ONE element changed.
   For Test 2: Control = Test 1 winner. Variant = Test 1 winner with ONE new element changed.
   This ensures each test's control is the optimized version from the prior test.

6. **Flag any untestable combinations**
   Some variables can't be cleanly isolated (e.g., a talking-head video hook can't be isolated from the talent change). Flag these and suggest the best available approach.

7. **Estimate total testing timeline**
   Given minimum spend per test and available daily budget, estimate how long the full isolation sequence will take. Flag if the timeline exceeds the client's testing window.

---

## Output Requirements

**Variable Audit**
Complete inventory of all changing elements between control and proposed variant, with isolation status: Isolated / Needs Separation.

**Isolation Sequence**
Test 1 → Test 2 → Test 3: each with control description, variant description, variable being isolated, and success metric.

**Timeline Estimate**
Based on budget and estimated duration per test, total time to complete the isolation sequence.

**Shortcut Option** (when applicable)
If full isolation is not feasible within budget or timeline, document the minimum viable isolation approach: which one test to run first to get the most learning from limited resources.

---

## Best Practices Applied

- One variable per test is the non-negotiable rule — every deviation from this produces uninterpretable data
- The highest-impact variable is always tested first to maximize learning velocity
- Each subsequent test uses the winner of the prior test as its control — isolation sequences compound
- "New creative" tests (where everything changes) are valid as proof-of-concept runs but must be labeled as such, not treated as variable tests
- Untestable combinations are acknowledged honestly rather than forced into an invalid structure

---

## Guardrails

- Do not approve a test where more than one variable changes — always restructure first
- Do not sequence tests in random order — always prioritize by impact on primary metric
- Do not use the original control for Test 2 if Test 1 produced a winner — that invalidates the sequence
- Do not label a multi-variable "creative refresh" as a proper A/B test
- Do not assume a confounded test result tells you anything definitive — flag ambiguity explicitly

---

## Example Requests

1. "We want to test a new creative where we're changing the hook, adding a testimonial, switching from a static to a video, and updating the CTA. How do we isolate this properly?"

2. "We ran a test last month where the variant had a different hook, headline, and visual. It won by 35%. We don't know what drove the result. Help us figure out what to test next to isolate the driver."

3. "Here's our current winning ad. We want to iterate on it in 5 ways. Build me a proper isolation sequence so we're always testing one thing at a time."
