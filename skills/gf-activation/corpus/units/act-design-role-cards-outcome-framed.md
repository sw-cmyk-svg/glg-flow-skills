---
id: act-design-role-cards-outcome-framed
stage: activation
sub_stage: signup
business_model: plg-saas
tactic_family: personalization
unit_type: case-study
metric: [activation_rate, time_to_activation]
provenance: public
sources:
  - "AI UX Playground — AI onboarding compared: Notion AI, Lovable, Manus (Jul 2026). https://aiuxplayground.com/teardowns/compare/ai-onboarding-first-value"
---
**Case study — Manus: outcome-framed role cards that point at a first task.**

Manus opens its signup with a **9-card role grid**, but the cards are framed by **what the user
wants to get done** (outcomes/jobs), not by job title or demographic — and tapping a card both
captures identity and **points the user at a first task**. This is a different personalization
move from a data-collection survey ([[act-tactic-segment-at-signup]]): the segmentation choice
*is* the first step toward value.

**The design lesson.** If you segment at entry, frame the choices as **outcomes** ("I want to
build X") rather than roles ("I'm a PM"), and make the selection advance the user toward doing
the thing — tapping a card moves the flow (no separate Next button).

**When it applies.** Products with distinct use-cases where the entry choice can seed the first
task (builders, assistants, multi-template tools). Overkill for single-use-case products.

**Caution.** The teardown reports **no activation metrics** — design pattern, not benchmark.
Keep the choice **skippable**: Manus's own skip is "easy to miss," which shades toward a dark
pattern — offer a clear skip so the segmentation never becomes a forced gate
([[act-principle-make-it-easy-friction]]). Pairs with [[act-framework-onboarding-shape]].
