# A/B Test Matrix Creator

**Category:** testing
**Tier:** pro

## Purpose

This Skill builds a complete, structured A/B test matrix for a creative program — a prioritized grid of all planned tests, their variables, their controls, their hypotheses, and their sequencing logic. Rather than testing reactively, teams with a test matrix run a systematic creative program where every test generates data that informs the next test. This Skill turns isolated tests into a learning machine.

---

## When to Use

- You're planning a new creative testing quarter and need a structured testing roadmap
- You have multiple hypotheses and need to sequence them intelligently
- You want to ensure tests don't interfere with each other (same variable tested simultaneously)
- A client or stakeholder wants to see a structured testing plan before budget approval
- You've just launched a new product or offer and need a testing plan to find the winning creative formula
- You're building a test matrix from scratch for a new account

---

## Inputs Required

- List of creative hypotheses or ideas to test (3-10 minimum)
- Current top-performing creative (the control baseline)
- Available monthly test budget
- Campaign objective (conversions, leads, traffic, etc.)
- Average CPC and CVR for benchmark estimation
- Testing timeline (e.g., 4 weeks, 8 weeks, 1 quarter)
- Audience structure (single audience per test, or multiple audiences tested simultaneously?)
- Optional: existing test history (what has already been tested)

---

## What This Skill Does

Organizes hypotheses into a sequenced testing matrix with: test number, variable being tested, control, variant, hypothesis, success metric, minimum spend, estimated test duration, test dependencies, and logical sequencing based on the insight hierarchy (hooks first, then offer, then format, then proof, then CTA).

---

## Analysis Workflow

1. **Audit the hypothesis list**
   Review all submitted hypotheses. Flag any that are confounded (multiple variables) or insufficiently defined. Prompt for refinement before including in the matrix.

2. **Apply the insight hierarchy for sequencing**
   Order tests by which variable provides the most foundational learning first:
   - Layer 1: Hook and opening line (highest impact on CTR — test first)
   - Layer 2: Offer framing (highest impact on CVR — test second)
   - Layer 3: Format/creative type (biggest structural change — test when layers 1-2 are settled)
   - Layer 4: Proof element (testimonial vs. stat vs. before-after)
   - Layer 5: CTA variation
   - Layer 6: Visual direction (once copy structure is proven)

3. **Identify test dependencies**
   Some tests can only be meaningful after another test resolves. Example: testing proof type is premature if the hook hasn't been optimized. Flag dependencies and enforce sequencing.

4. **Estimate test budget and duration**
   For each test: estimate minimum spend for signal based on target CPC and CVR. Estimate duration based on daily budget. Flag any tests that won't reach valid spend within the testing window.

5. **Check for variable conflicts**
   If two tests change similar variables (e.g., both testing hook style), they must run sequentially, not simultaneously — concurrent tests on similar variables contaminate each other's data.

6. **Assign test priority scores**
   Score each test on three dimensions: (a) potential impact on primary metric, (b) ease of execution, (c) learning value. Tests scoring high on all three go first.

7. **Build the test matrix**
   Construct the full table with all test attributes. Include a "depends on" column to document sequencing logic visibly.

8. **Write the testing calendar**
   Map each test to a specific week or date window based on estimated duration and sequencing dependencies. Visualize as a timeline or Gantt-style table.

---

## Output Requirements

**Test Matrix Table**
| Test # | Variable | Control | Variant | Hypothesis | Success Metric | Min Spend | Est. Duration | Depends On | Priority |

**Testing Calendar**
Week-by-week or date-mapped schedule showing which tests run when.

**Budget Allocation Summary**
Total testing budget broken down by test, with any budget warnings for tests that may not reach signal.

**Sequencing Rationale**
A short explanation of why the matrix is ordered the way it is — what insight hierarchy logic governs the sequence.

---

## Best Practices Applied

- Tests are sequenced from foundational variables to downstream variables (hook before offer before format)
- Variable conflicts are identified and prevented before they contaminate data
- Budget realism is enforced — every test must have sufficient spend to be readable
- Test matrix is a living document — annotated with results as tests complete
- Tests that depend on prior results are clearly linked, not scheduled independently

---

## Guardrails

- Do not run tests on variables that haven't been isolated — confounded tests produce uninterpretable results
- Do not schedule more simultaneous tests than the budget can support (tests compete for spend)
- Do not build a matrix without a defined control — all tests need a baseline to compare against
- Do not prioritize easy-to-make tests over high-impact tests — execution ease is a secondary factor
- Do not treat the test matrix as permanent — it should be updated weekly as results come in

---

## Example Requests

1. "I have 8 creative hypotheses I want to test this quarter with a $5,000/month test budget. Build me a structured test matrix with sequencing and a calendar."

2. "We're launching a new product next month. We have no data yet. Build a testing plan from scratch that starts with the most foundational variables and works toward the most specific ones."

3. "Here's our current test matrix from last quarter with results. Update it for next quarter, remove completed tests, add 5 new hypotheses I want to include, and re-sequence based on what we learned."
