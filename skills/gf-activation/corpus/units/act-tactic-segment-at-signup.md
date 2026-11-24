---
id: act-tactic-segment-at-signup
stage: activation
sub_stage: signup
business_model: plg-saas
tactic_family: personalization
unit_type: tactic
metric: [activation_rate, time_to_activation]
provenance: public
sources:
  - "UserGuiding — How Top AI Tools Onboard New Users (2026). https://userguiding.com/blog/how-top-ai-tools-onboard-new-users"
---
**Tactic — ask a few segmenting questions at signup, then actually branch on them.**

Modern signup flows collect a little context to tailor what comes next. Across the 10 AI
tools UserGuiding reviewed, signup asked **3–5 questions**, most often **use case (7/10)**,
**role (6/10)**, and **purpose (5/10)**; Claude frames this as a conversational welcome survey
rather than a form.

**How to apply.** Ask only the 1–3 questions whose answers **change the first-value path**
(which template loads, which example data, which first action you point to). Then branch on
them — a role or use-case answer should visibly reshape the first screen, not just populate a
CRM field.

**When it applies.** Products with distinct user types or jobs-to-be-done, where a generic
first-run would under-serve most people. Less useful for single-use-case tools.

**Caution.** Collecting segmentation data is **not** the same as acting on it — the
UserGuiding teardown documents the *questions*, not confirmed downstream branching, and an
unused question is pure friction (see [[act-principle-make-it-easy-friction]]). Every question
must earn its place by changing what the user then sees. Pairs with
[[act-tactic-value-before-signup]].
