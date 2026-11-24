---
id: ret-principle-relevance-decay
stage: retention
sub_stage: engagement
business_model: plg-saas
tactic_family: personalization-relevance
unit_type: principle
metric: [w4_retention, weekly_active_users]
provenance: public
sources:
  - "General PLG personalization practice (Userpilot / Pendo / Amplitude personalization + behavioral-cohort material in hand); Fogg prompt-relevance."
---
**Principle — personalization is not set-once; relevance decays as the user's needs change.**

A product tuned to who the user was at signup slowly drifts out of step with who they are three
months in — new goals, new workflows, a different role, a maturing use case. Personalization that
never updates becomes **stale**, and stale experiences feel generic, which is the opposite of the
point. The durable version personalizes off **current behaviour and lifecycle stage**, not just the
static attributes captured at registration.

**How to apply.** Base tailored experiences on what the user is doing **now** — recent actions,
current lifecycle stage, evolving segment — and refresh them as behaviour shifts. Re-segment
periodically rather than freezing a user in their signup profile. Tie relevance to the moment (the
Fogg prompt lands only when it's relevant — [[ret-principle-fogg-behavior-model]]).

**When it applies.** Products used over months where the user's needs evolve; multi-persona or
multi-use-case products where one static profile can't stay accurate.

**Caution (ethics + honesty).** Personalization draws on user data — keep it within the client's
**aggregate / consented** data boundary, be transparent about what drives it, and let users correct or
opt out. Over-personalization reads as **creepy** ("how do they know that?") and can trap users in a
narrow view; keep it helpful, not surveillant. Pairs with [[ret-tactic-behavioral-segmentation]] and
[[ret-tactic-next-best-action]].
