# Test Priority Ranker

**Category:** testing
**Tier:** pro

## Purpose

This Skill takes a backlog of creative test ideas or hypotheses and outputs a prioritized testing queue based on a structured scoring model. It prevents the two most common prioritization mistakes in creative testing: running the easiest tests instead of the highest-impact tests, and running too many tests simultaneously without a clear order of precedence. Every test in the backlog gets a score and a position in the queue.

---

## When to Use

- You have more test ideas than budget or time to run them all
- Your creative team disagrees on what to test next
- You need to justify a testing priority decision to a client or stakeholder
- You've completed a round of tests and need to plan the next round from a backlog
- You want a defensible, systematic process for deciding test order across multiple campaigns

---

## Inputs Required

- Backlog of test ideas or documented hypotheses (3-20 items)
- Primary metric being optimized for this account (CTR, CVR, ROAS, CPL, etc.)
- Current performance gap to goal (how far is performance from target?)
- Available testing budget per week or month
- Any tests that are time-sensitive (promotional deadlines, seasonal relevance)
- Optional: existing test results that inform the relative importance of variables

---

## What This Skill Does

Scores every test in the backlog on four dimensions — potential impact, evidence strength, execution effort, and learning value — then combines scores into a priority ranking with position in queue, estimated start date, and brief rationale for each placement.

---

## Analysis Workflow

1. **Standardize the test backlog**
   Ensure every item in the backlog is described with: the variable being tested, the expected direction of impact, and the target metric. Items that are too vague to score are flagged for refinement.

2. **Score each test on Dimension 1: Potential Impact**
   How much could this test improve the primary metric if it wins?
   - High (3 pts): Testing a variable with direct, large influence on the primary metric (e.g., hook for CTR, offer for CVR)
   - Medium (2 pts): Testing a variable with moderate influence (e.g., proof type, visual style)
   - Low (1 pt): Testing a variable with peripheral influence (e.g., CTA button text, color)

3. **Score each test on Dimension 2: Evidence Strength**
   How strong is the rationale for this test?
   - Strong (3 pts): Supported by account data, customer language, or a confirmed pattern from past tests
   - Directional (2 pts): Supported by industry benchmarks or general DR principles
   - Weak (1 pt): Based on intuition or copying a competitor without account-specific evidence

4. **Score each test on Dimension 3: Execution Effort**
   How much production work is required to run this test?
   - Low effort (3 pts): Copy change only, or minimal design edit
   - Medium effort (2 pts): New static design or short copy rewrite
   - High effort (1 pt): New video shoot, major redesign, or complex production

5. **Score each test on Dimension 4: Learning Value**
   How much will a definitive result from this test tell us about the account's winning formula?
   - High (3 pts): Resolves a foundational question about what drives performance
   - Medium (2 pts): Adds to an existing pattern with incremental value
   - Low (1 pt): Tactical optimization with limited generalizable learning

6. **Calculate total priority score**
   Total = Impact + Evidence + Execution + Learning (max 12 pts). Sort descending.

7. **Apply time-sensitive overrides**
   Any test tied to a promotional deadline or seasonal window is elevated regardless of score — flag with "(Time Override)" in the queue.

8. **Build the prioritized testing queue**
   Output ranked list with score breakdown, recommended start date, estimated duration, and one-line rationale for each placement.

---

## Output Requirements

**Prioritized Test Queue**
| Rank | Test | Impact | Evidence | Effort | Learning | Total Score | Start Date | Rationale |

**Queue Summary**
- Top 3 tests to run immediately
- Tests to hold for next round (lower priority)
- Tests to drop or deprioritize (low score with no time pressure)
- Time-sensitive tests elevated above their score

**Budget Allocation Recommendation**
How to distribute available testing budget across the top 3-5 tests in the queue.

---

## Best Practices Applied

- Impact on primary metric is the highest-weighted dimension in practice
- Evidence strength prevents "gut feel" tests from crowding out data-informed tests
- Execution effort is scored as a tiebreaker, not a primary driver — don't optimize for easy tests
- Learning value ensures the test program builds compounding knowledge, not just individual data points
- Time-sensitive overrides are documented transparently so the team understands why the queue shifted

---

## Guardrails

- Do not allow execution ease to dominate the ranking — low-effort tests belong at the bottom if impact is low
- Do not deprioritize high-impact tests simply because they require more production
- Do not run more than 3-4 tests simultaneously — parallel tests compete for budget and confuse the data
- Do not treat the score as absolute — document any human judgment overrides with explicit rationale
- Do not skip the time-sensitive override check — missing a seasonal window can eliminate an entire learning opportunity

---

## Example Requests

1. "I have 12 test ideas and can only run 3-4 at a time this month. Score them and tell me exactly which ones to run first and why."

2. "Our client wants to test everything at once. Help me build a prioritized testing queue I can show them to explain why some tests need to wait."

3. "We just finished a test round. Here's the results and our backlog of next ideas. Rescore the backlog based on what we learned and give me an updated priority ranking."
