---
id: act-design-embedded-prompt-starters
stage: activation
sub_stage: onboarding
business_model: plg-saas
tactic_family: guidance
unit_type: case-study
metric: [activation_rate, time_to_activation]
provenance: public
sources:
  - "AI UX Playground — Notion AI onboarding teardown. https://aiuxplayground.com/teardowns/notion/onboarding"
---
**Case study — Notion AI: embedded first value via categorized prompt starters.**

Notion AI has **no empty chat screen and no AI home**. AI is invoked from the editor where the
cursor already sits, context is implicit (the current page/block/selection is what "summarize
this" acts on), and output inserts straight into the doc. For the first run, it surfaces
**prompt starters grouped by job** — write, edit, summarize — each a **complete, editable
sentence that runs in one click** (e.g. "Write meeting agenda"), which both yields a first
success and teaches good prompting by example.

**The design lesson.** When your product *extends a surface the user already has open*, reach
first value **in place** rather than routing them through a separate flow. Group starters by
the user's intent (job-to-be-done), not by model feature; label buckets by job or they read as
noise.

**When it applies.** AI (or any assistive feature) layered onto an existing workspace/editor.
Less applicable to standalone products with their own blank canvas (see the wizard branch in
[[act-framework-onboarding-shape]]).

**Caution.** The teardown reports **no metrics** — treat this as a *design pattern*, not a
benchmark. Its own trade-off: discoverability rests entirely on editor affordances, so
first-timers may not know AI exists until they invoke it, and selection scope is opaque. Pairs
with [[act-design-embedded-cues-over-tours]] and [[act-principle-make-it-easy-friction]].
