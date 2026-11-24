# Galangal Flow — growth specialist skills (public sampler)

[![Install as a Claude Code plugin](https://img.shields.io/badge/Claude_Code-install_plugin-d97757?logo=anthropic&logoColor=white)](#install)
[![License: MIT](https://img.shields.io/badge/License-MIT-blue.svg)](LICENSE)

Six installable [Claude skills](https://docs.claude.com/en/docs/claude-code/skills), packaged as
one plugin, that turn Claude into a **scope-disciplined, evidence-grounded growth specialist**
instead of a general chat. This is the **public PLG-SaaS sampler** — it shows the method; it is not
the full product.

- **`gf-diagnose`** — diagnoses a growth funnel from **aggregate-only** weekly CSVs (funnel /
  retention / revenue): validates the measurement framework first, surfaces leaks as *candidates for
  a human to confirm* (never verdicts), sizes them against benchmarks, cites every finding.
- **`gf-activation`** — arrival → first value ("aha"): onboarding, time-to-value, activation rate.
- **`gf-retention`** — after first value: habit, stickiness, churn, re-engagement / win-back.
- **`gf-monetization`** — usage → revenue: pricing, packaging, paywalls, free-to-paid, expansion.
- **`gf-acquisition`** — the right new users: channels, CAC, paid vs organic, PLG/viral loops.
- **`gf-referral`** — users as a source of users: refer-a-friend, two-sided rewards, reviews/UGC.

Each AARRR specialist **scopes the question first**, routes off-scope asks to the right neighbour,
grounds every recommendation in a bundled, cited corpus, and is honest about weak evidence. They pair
with `gf-diagnose` for the data-analysis step.

## What this is (and isn't)

**Is:** the general PLG-SaaS version, grounded in a **public** knowledge base, so you can feel the
difference vs. a blank chat — right frame, cited claims, scope discipline, honesty about uncertainty.

**Isn't:** a certified client instance. The proprietary layer — the regulated **archetype overlays**
(digital bank/wallet, betting, e-commerce), the full corpus, the live-data connector with its enforced
data boundary, and the done-for-you stamping/handoff — is not in this sampler. On a regulated vertical
this public corpus is deliberately thin, and the skills say so.

**Data boundary:** these skills work on **aggregates only** — weekly rollups, never user-level rows.
Paste user-level data and `gf-diagnose` will stop and ask you to re-export as weekly aggregates.

## Install

### As a plugin (recommended)

```bash
claude plugin marketplace add sw-cmyk-svg/glg-flow-skills
claude plugin install glg-flow-growth-specialists@glg-flow
```

### Or copy the skills directly

```bash
git clone https://github.com/sw-cmyk-svg/glg-flow-skills
cp -R glg-flow-skills/skills/* ~/.claude/skills/
```

Either way, invoke a specialist explicitly (`/gf-diagnose`, `/gf-activation`, …) or just describe the
task and Claude will trigger the right one.

*(To use in a claude.ai Project instead: create a Project, paste a `SKILL.md` body as custom
instructions, and upload that skill's bundled `knowledge/` or `corpus/` files as Project knowledge.)*

## Try it in 30 seconds

**Diagnose a PLG funnel** — `examples/sample-plg-funnel.csv` has a signup→activation drop over the
last weeks. Paste it and say *"diagnose this."* You should get a plain-language read that flags any
data issues first, surfaces the activation decline as a soft candidate, sizes it against the bundled
benchmarks, and cites cards by id — not a confident verdict. (`examples/sample-weekly-funnel.csv` is
an e-commerce-shaped funnel for contrast — the diagnose knowledge base is PLG-SaaS, so it will tell
you honestly when no benchmark card fits a given step.)

**Ask a specialist** — e.g. gf-activation: *"users sign up but don't reach first value — fix our
onboarding."* You get a scoped answer that first pins down your "aha" moment and checks it's actually
an activation problem, then cited recommendations with honesty caveats. Try an off-scope question
(*"which ad channels should we cut?"*) and watch it route you to the Acquisition specialist instead.

## What's inside

```
.claude-plugin/
  plugin.json          # plugin manifest
  marketplace.json     # marketplace entry (claude plugin marketplace add)
skills/
  gf-diagnose/         SKILL.md + knowledge/ (cited cards) + spec/ + HARD-RULES.md
  gf-activation/       SKILL.md + corpus/ (29 units) + reference/ (framework, guardrails, spec)
  gf-retention/        SKILL.md + corpus/ (19 units) + reference/
  gf-monetization/     SKILL.md + corpus/ (18 units) + reference/
  gf-acquisition/      SKILL.md + corpus/ (18 units) + reference/
  gf-referral/         SKILL.md + corpus/ (19 units) + reference/
examples/
  sample-plg-funnel.csv
  sample-weekly-funnel.csv
LICENSE
```

Every knowledge card and corpus unit carries its own `provenance` and `sources` — this is **public,
cited evidence**, not model memory.

## License

MIT — see [`LICENSE`](LICENSE). Use, modify, and redistribute freely; the bundled knowledge cards and
corpus units are public, cited evidence.

---
*Galangal Flow is a per-client growth-OS assembly kit. This repo is the open sampler of its method.
Full archetype overlays + certified instances are delivered per engagement.*
