---
id: act-design-embedded-cues-over-tours
stage: activation
sub_stage: onboarding
business_model: plg-saas
tactic_family: guidance
unit_type: case-study
metric: [activation_rate, time_to_activation]
provenance: public
sources:
  - "UserGuiding — How Top AI Tools Onboard New Users (2026). https://userguiding.com/blog/how-top-ai-tools-onboard-new-users"
verified: 2026-11-17
---
**Design pattern — guide with embedded cues, not tooltips and checklists.**

In UserGuiding's 2026 review, **only 4 of 10 top AI tools still use tooltips/checklists**;
most guide via cues built into the interface itself. Observed patterns:

- **Example prompts in the empty state** — Perplexity gives new users starter prompts so
  they act without reading a guide.
- **Templates / ready-made defaults** — ElevenLabs reduces cognitive load so users start
  from a working example rather than a blank canvas.
- **In-context copilot** — HeyGen's avatar delivers tutorial messages during the task
  (learn-by-doing), not before it.

**How to apply (Design step output).** Replace a multi-step tour with: a non-empty first
screen (templates/examples), one obvious first action, and just-in-time hints at the point
of need. Wireframe intent: *empty state → seeded example → first result → light nudge to
the next action.*

**When it applies.** Strong for products with an open-canvas or prompt surface. A
guided checklist can still beat embedded cues when activation requires a fixed multi-step
setup (connect data → invite team → configure).

**Related.** [[act-benchmark-tour-completion-by-steps]] (why long tours leak),
[[act-principle-time-to-value]].
