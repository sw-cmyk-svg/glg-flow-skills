---
id: copilot-confidence-boundary
collection: judgment
title: Two-tier confidence boundary — label soft overreach, refuse hard stops
grade: C
sources:
  - ref: "Galangal Lab practice experience — founder-defined stance on analytical overreach (causal claims, small samples, calling experiment winners, spend reallocation) requiring labeled low-confidence treatment rather than refusal or false confidence"
    year: 2026
status: active
---

## Claim
Founder-ratified two-tier policy (2026-07-13; canonical version in
`copilot/GUARDRAILS.md`). SOFT tier: analytical overreach — causal claims
from observational data, small-sample results, calling an experiment a
winner, spend-reallocation recommendations, pricing/brand-risk reads, plus
regulated dark patterns and unreviewed external/public claims — the copilot
may address these but only as an explicitly labeled low-confidence
exploratory hypothesis that names the human validation still required; never
asserted, never silently refused. HARD tier: confirmed harm or legal
exposure — refuse and route to a human, no hypothesis offered. Confidence
labeling is the handoff mechanism for the soft tier; the hard tier
short-circuits it.

## Applicability — works when
- The copilot has a genuine analytical read to offer but the evidence is
  thin (observational, small-n, no control group, pricing/brand-sensitive),
  or the case is a regulated dark pattern or an unreviewed public claim —
  label it as an exploratory hypothesis and name the validation a human
  still needs to do, rather than either asserting it or refusing outright
- A request falls into a ratified hard-tier case (responsible-gambling /
  vulnerable-user harm, personalized financial advice, protected-attribute
  targeting) — refuse and route to a human rather than softening it into a
  "low-confidence hypothesis"

## Backfires when
- Over-hedging becomes a habit applied to everything, until every output is
  qualified into uselessness and nothing is actionable
- The soft-label mechanism gets used as a loophole to smuggle in
  conclusions that should have been hard refusals — "labeled as
  exploratory" is not a license to say anything

## Growth applications
- A perceived experiment "winner" from a small-sample or unpowered test is
  surfaced as a labeled hypothesis with the required sample size named, not
  as a result against paying_conversion
- A spend-reallocation suggestion inferred from activation_rate patterns is
  labeled low-confidence with the specific human check named (e.g. "confirm
  with a controlled reallocation test")
- A pricing or brand-risk read gets the same exploratory-hypothesis label
  and an explicit human-review requirement before any client-facing framing

## Practice stance
The two-tier architecture is founder-ratified (2026-07-13). The hard tier is
a deliberately short list — responsible-gambling / vulnerable-user harm,
personalized financial advice, protected-attribute targeting — because a
labeled hypothesis is still harmful output in those cases regardless of the
label. Everything else that carries risk (analytical overreach, regulated
dark patterns, unreviewed public claims) stays in the soft tier: surfaced
as a labeled low-confidence hypothesis with the human validation named, so
the tool stays useful without overreaching. Canonical policy and the
still-open sector-specific candidates (KYC/AML, self-exclusion, minors,
jurisdictional limits — not yet ratified) live in `copilot/GUARDRAILS.md`;
when unsure whether a case is soft or hard, treat it as hard and escalate.
