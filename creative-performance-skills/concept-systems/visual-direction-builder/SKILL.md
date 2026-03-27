# Visual Direction Builder

**Category:** concept-systems
**Tier:** pro

## Purpose

This Skill generates specific, actionable visual direction notes for ad creative — detailed enough to hand to a designer, a UGC creator, or paste directly into an AI image generation tool. "Lifestyle photo" is not a visual direction. This Skill produces directions that describe talent, environment, action, mood, color treatment, composition, and text overlay — everything needed to produce the intended visual without a follow-up briefing call.

---

## When to Use

- You're briefing a designer on static ad visuals and need specificity beyond "make it look good"
- You're using an AI image generation tool (Midjourney, DALL-E, Adobe Firefly) and need detailed prompts
- You're briefing a UGC creator and want to give them specific visual direction beyond the script
- You're building a creative concept and need the visual component to match the copy angle precisely
- You want to test different visual treatments for the same copy and need distinct visual directions for each
- You're building a style guide for ad creative

---

## Inputs Required

- Ad concept or copy angle (what the ad is about, what it's trying to do)
- Product description (what it looks like, what it does)
- Target audience (who should appear in or relate to the visual)
- Platform and format (Meta Feed, Reels, Stories — affects aspect ratio and style)
- Tone / aesthetic target (authentic UGC, polished studio, editorial, raw lifestyle, minimalist, bold graphic)
- Any brand visual rules (colors, logo usage, fonts)
- Optional: visual references or competitor examples to emulate or differentiate from

---

## What This Skill Does

Generates 3-5 complete visual direction specifications for an ad concept, each targeting a different aesthetic treatment. Each direction is specific enough for direct execution by a designer, photographer, creator, or AI tool — without additional clarification required.

---

## Analysis Workflow

1. **Extract the emotional job of this visual**
   What emotion should the visual activate? Trust, aspiration, curiosity, urgency, empathy, excitement? The visual's job is to amplify the copy's primary emotion, not decorate it.

2. **Identify the visual's entry point**
   What should the viewer's eye land on first? Product in use, human face, text overlay, environmental detail? The visual hierarchy must support the ad's primary message.

3. **Define talent parameters**
   If a person appears: approximate age, apparent ethnicity and gender (when relevant to the product and audience), expression type (candid and natural vs. direct camera address), energy level (high, neutral, warm), and what they are doing in the scene.

4. **Define the environment**
   Where is this scene set? Be specific: "a bright, moderately tidy kitchen counter with a coffee maker in the background" not "kitchen setting." The environment signals lifestyle context and aspirational or relatable tone.

5. **Define the action**
   What is happening in the image or video frame? Passive (product sitting, person smiling) or active (product being used, before/after reveal, reaction moment)? Active visuals outperform passive in most paid social contexts.

6. **Define the production aesthetic**
   Choose and specify: Studio polished / Lifestyle editorial / Authentic UGC / Raw/handheld / Flat lay product / Screen recording / Text-card / Graphic/illustrated. Each aesthetic signals a different relationship between brand and audience.

7. **Define text overlay direction** (if applicable)
   Position, font weight (bold vs. light), color contrast against background, hook text to display on image/video, any animation or reveal effect.

8. **Write the AI image prompt version**
   Translate the visual direction into a structured AI prompt format usable in Midjourney, DALL-E, or Firefly. Include: subject, action, setting, lighting, style, mood, aspect ratio.

9. **Write 3-5 distinct visual direction variants**
   Variant A: Polished aspirational
   Variant B: Authentic UGC style
   Variant C: Product-forward clean
   Variant D: Problem-state contrast (before)
   Variant E: Social proof/evidence visual

---

## Output Requirements

**Visual Direction Specifications (3-5 variants)**

For each variant:
```
VISUAL DIRECTION: [Variant Name]
FORMAT: [Aspect ratio + platform]
AESTHETIC: [Style descriptor]
EMOTION TARGET: [What the viewer should feel]

SHOT DESCRIPTION:
  Talent: [Age, expression, action, energy — or "no talent, product only"]
  Environment: [Specific setting with details]
  Action: [Exactly what is happening]
  Composition: [Where the eye lands first, framing notes]
  Lighting: [Natural/warm/cool/dramatic — specific style]
  Color treatment: [Warm/cool/neutral/brand-specific]

TEXT OVERLAY (if applicable):
  Hook text: [Exact text]
  Position: [Top/center/bottom]
  Style: [Bold/clean/minimal]

AI IMAGE PROMPT:
  [Full structured prompt ready to paste]

DESIGNER NOTES:
  [Any additional execution guidance]
```

---

## Best Practices Applied

- Visual direction is specific enough to prevent misinterpretation — "realistic photo of" not "good-looking photo"
- The visual's emotional job is always defined before the visual details are specified
- Production aesthetic is chosen deliberately to match the awareness stage and target audience's trust level
- Text overlays in ads are treated as part of the visual direction, not afterthoughts
- AI prompts are structured to produce usable outputs, not aspirational descriptions

---

## Guardrails

- Do not write visual directions that require more production than the brief's budget or timeline allows
- Do not describe talent in ways that create stereotyping or demographic exclusion problems
- Do not write "generic smiling person" as a talent direction — specificity is required
- Do not design visuals that contradict the copy's emotional register
- Do not write visual directions that ignore platform specifications (9:16 for Reels, 1:1 for Feed, etc.)

---

## Example Requests

1. "We're creating 3 different visual treatments for the same ad copy. Give me specific visual directions for: (1) a polished lifestyle version, (2) an authentic UGC version, and (3) a text-card version."

2. "I need to paste visual direction into Midjourney for 5 ad concepts. Write the AI prompts plus the human-readable direction for a designer so both versions are ready."

3. "Our current ad visuals are generic stock photos. Give me 4 specific visual directions that are more authentic and on-brand, specific enough for our design team to execute without a briefing call."
