# Creative Performance Skills for Claude Code

## Overview

This repository is a modular creative operating system for performance advertising, built as a Claude Code Capabilities library. It is not a swipe file, a prompt generator, or a brainstorming tool. It is a structured, operator-grade creative infrastructure system engineered to help performance teams diagnose, plan, generate, test, and report on ad creative with direct-response rigor. Every Skill in this system was designed around a specific job a performance creative team needs to complete — from killing underperforming concepts to generating 100+ categorized ad concepts across 17 proven Meta formats.

---

## What This Repository Includes

### Creative Diagnosis
Tools to classify creative as Kill, Fix, or Scale based on real performance evidence. Includes fatigue detection, postmortem analysis, and winner pattern extraction.

### Testing Systems
Hypothesis-first A/B testing infrastructure. Builds structured test plans with testable variables, success metrics, and prioritized test queues — no guesswork.

### Messaging Systems
Maps creative angles to audience awareness stages. Converts voice-of-customer language into hooks. Writes objection-led copy and full direct-response body copy.

### UGC Systems
Generates usable UGC briefs for creators or internal teams with scene direction, delivery notes, proof points, and CTAs. Includes creator instructions, testimonial structures, and iteration plans.

### Reporting
Creative performance reports built for decision-making, not decoration. Generates stakeholder summaries, concept performance reports, and format-level analysis.

### Landing Page Alignment
Diagnoses message mismatch between ads and landing pages across five continuity dimensions: promise, offer, emotion, objection handling, and CTA.

### Concept Generation
Meta format-based concept engine that produces 100+ categorized ad concepts across 17 proven formats. Includes headline generators, visual direction builders, and format batch testing planners.

### Reusable Templates
Brand brief, creative intake, offer input, and audience research templates that feed every other Skill in one shot.

---

## Who This Is For

- Paid social operators managing Meta, TikTok, or multi-platform campaigns
- Creative strategists responsible for brief-to-launch workflow
- Media buyers who need to move faster from data to decision
- Founders running their own paid acquisition
- Agencies managing creative across multiple client accounts
- Growth marketers building and scaling acquisition systems
- Performance creative teams building concept libraries
- In-house creative leads who need to structure testing programs

---

## What Problems This Solves

**Creative is killed or scaled on instinct, not evidence.**
The diagnostics system eliminates that. Kill/Fix/Scale decisions are made on structured criteria from real performance data.

**A/B tests are run without hypotheses.**
The testing system forces hypothesis-first thinking with variable isolation, rationale documentation, and defined success metrics.

**Hooks are generic because they're not built from real customer language.**
The VOC Hook Builder turns reviews, comments, sales calls, and testimonials into specific, psychologically loaded hooks.

**UGC briefs are vague and creators produce unusable content.**
The UGC system generates scene-by-scene briefs with delivery style, hook scripts, filming notes, and explicit CTA instructions.

**Creative reports are long, unfocused, and don't drive decisions.**
The reporting system produces short, scannable reports structured around Kill/Fix/Scale signals and next recommended actions.

**Ads and landing pages say different things.**
The landing page alignment system audits all five continuity dimensions between ad promise and landing page delivery.

**Ad concepts are random and untestable.**
The concept engine generates 100+ concepts organized by format and awareness stage so teams can run structured category tests, not random experiments.

---

## How to Use These Skills

Each Skill lives in its own folder and contains a `SKILL.md` file. To install any Skill into Claude Code:

1. Open Claude Code in your project directory
2. Navigate to the Skill folder you want to install
3. Copy the `SKILL.md` contents into your Claude Code Skills configuration, or reference it directly as a system-level Skill
4. Provide the required inputs listed in the Skill's **Inputs Required** section
5. Run the Skill by describing the job you need done

Most Skills are designed to work from user-provided inputs only — no API access required unless specified.

---

## Input Types These Skills Work Best With

- Creative performance exports (CTR, CPC, ROAS, frequency, CPM, hook rate, hold rate)
- Ad screenshots or copy text
- Landing page URLs or HTML
- Customer reviews (Amazon, Google, Trustpilot, G2, Capterra)
- Survey responses and customer interviews
- Sales call notes and objection logs
- Reddit threads and community forum posts
- Founder notes and positioning documents
- Product pages and feature lists
- Offer descriptions and pricing structures
- Existing ad copy and creative concepts
- Creative test history and test results
- Competitor ad examples

---

## Repository Structure

```
/creative-performance-skills/
  README.md
  /creative-diagnostics/
    /kill-fix-scale-diagnostician/         SKILL.md
    /fatigue-pattern-reviewer/             SKILL.md
    /creative-postmortem-analyzer/         SKILL.md
    /winner-pattern-extractor/             SKILL.md
  /testing/
    /hypothesis-builder/                   SKILL.md
    /ab-test-matrix-creator/               SKILL.md
    /variable-isolation-planner/           SKILL.md
    /test-priority-ranker/                 SKILL.md
  /messaging/
    /awareness-angle-mapper/               SKILL.md
    /voice-of-customer-hook-builder/       SKILL.md
    /objection-led-copywriter/             SKILL.md
    /direct-response-body-copy-generator/  SKILL.md
  /ugc/
    /ugc-brief-generator/                  SKILL.md
    /creator-instruction-builder/          SKILL.md
    /testimonial-structure-planner/        SKILL.md
    /ugc-iteration-planner/                SKILL.md
  /reporting/
    /creative-report-generator/            SKILL.md
    /stakeholder-summary-builder/          SKILL.md
    /concept-performance-reporter/         SKILL.md
  /landing-page-alignment/
    /ad-to-landing-gap-auditor/            SKILL.md
    /message-match-reviewer/               SKILL.md
    /offer-continuity-checker/             SKILL.md
  /concept-systems/
    /meta-format-concept-engine/           SKILL.md
    /headline-pattern-interrupt-generator/ SKILL.md
    /visual-direction-builder/             SKILL.md
    /format-batch-testing-planner/         SKILL.md
  /templates/
    /brand-brief-template/                 SKILL.md
    /creative-intake-template/             SKILL.md
    /offer-input-template/                 SKILL.md
    /audience-research-template/           SKILL.md
```

---

## The 17 Meta Creative Formats

Category-based testing is how serious performance teams run creative. Rather than testing isolated random ads, you test a complete format category — all 6 founder story concepts together, all 5 before/after concepts together — so you learn whether the format itself works for your audience and offer before iterating on variables within it.

| # | Format Name | Core Mechanism |
|---|---|---|
| 1 | Founder Story | Personal credibility narrative |
| 2 | Problem-Solution | Identify pain → deliver resolution |
| 3 | Before-After | State transformation proof |
| 4 | Testimonial | Third-party social proof |
| 5 | UGC Demo | Authentic in-use demonstration |
| 6 | Listicle | Scannable benefits or truths |
| 7 | Myth-Buster | Challenge false belief, insert truth |
| 8 | Comparison | Direct or implied contrast |
| 9 | Objection Crusher | Preempt and destroy resistance |
| 10 | Stat-Led Proof | Data-first credibility |
| 11 | Process Breakdown | Step-by-step how it works |
| 12 | Product Explainer | Feature-to-benefit translation |
| 13 | Review Montage | Aggregated social proof |
| 14 | Offer-Led Promo | Deal, urgency, and scarcity first |
| 15 | Day-in-the-Life | Lifestyle integration narrative |
| 16 | FAQ Style | Anticipate and answer objections |
| 17 | Mistake-Driven Angle | "Are you doing this wrong?" hook |

---

## Recommended First Installs

Install these 10 Skills first to build your core creative operating layer:

1. **brand-brief-template** — Feed every other Skill from one source of truth
2. **kill-fix-scale-diagnostician** — Make evidence-based creative decisions immediately
3. **awareness-angle-mapper** — Ensure creative is matched to the right awareness stage
4. **voice-of-customer-hook-builder** — Build hooks from real customer language
5. **hypothesis-builder** — Never run a test without a documented hypothesis
6. **meta-format-concept-engine** — Generate your first 100+ concept library
7. **ugc-brief-generator** — Brief creators with precision
8. **ad-to-landing-gap-auditor** — Stop losing conversions at the landing page
9. **creative-report-generator** — Report performance clearly to stakeholders
10. **direct-response-body-copy-generator** — Write body copy that converts

---

## Operating Philosophy

**Diagnosis before ideation.**
Before generating new concepts, understand why existing ones are winning or losing. Creative strategy starts with data, not brainstorming.

**Hypotheses before tests.**
Every A/B test must begin with a written hypothesis: what you believe, what variable you're isolating, why you believe it, and what metric proves it.

**Specificity over generic creativity.**
"A woman smiling at her phone" is not a visual direction. "A woman in her 30s, sitting at a kitchen island, phone tilted toward camera, genuine laugh reaction — not posed" is a visual direction.

**Direct-response structure over fluff.**
Hook → Agitate → Prove → CTA. This sequence exists because it converts. Every piece of copy in this system is built on it.

**Systemized iteration over random ad making.**
The most dangerous creative practice is making ads based on gut feel without a test structure. This system turns ad making into a repeatable, learnable, improvable process.

---

## Notes

These Skills do not require API access and operate entirely from user-provided inputs. Paste in your data, your copy, your customer reviews, your landing page, your offer — and the Skill will produce structured, operator-grade outputs. All Skills are designed to be run directly inside Claude Code with no external integrations required.
