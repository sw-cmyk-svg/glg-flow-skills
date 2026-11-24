# Galangal Flow — growth specialist skills (public sampler)

Two installable [Claude skills](https://docs.claude.com/en/docs/claude-code/skills)
that turn Claude into a **scope-disciplined, evidence-grounded growth specialist**
instead of a general chat. This is the **public PLG-SaaS sampler** — it shows the
method; it is not the full product.

- **`gf-diagnose`** — diagnoses a growth funnel from **aggregate-only** weekly CSVs
  (funnel / retention / revenue): validates the measurement framework first, surfaces
  leaks as *candidates for a human to confirm* (never verdicts), sizes them against
  benchmarks, and grounds every finding in a cited knowledge card.
- **`gf-activation`** — an activation & onboarding specialist (arrival → first value):
  scopes the question, routes off-scope asks to the right neighbour, and cites a curated
  corpus for every recommendation — honest about weak evidence.

## What this is (and isn't)

**Is:** the general PLG-SaaS version, grounded in a **public** knowledge base, so you can
feel the difference vs. a blank chat — right frame, cited claims, scope discipline, and
honesty about uncertainty.

**Isn't:** a certified client instance. The proprietary layer — the regulated **archetype
overlays** (digital bank/wallet, betting, e-commerce), the full corpus, the live-data
connector with its enforced data boundary, and the done-for-you stamping/handoff — is not
in this sampler. On a regulated vertical this public corpus is deliberately thin, and the
skills say so.

**Data boundary:** these skills work on **aggregates only** — weekly rollups, never
user-level rows. Paste user-level data and the skill will stop and ask you to re-export as
weekly aggregates.

## Install (Claude Code)

Copy each skill into your user skills directory:

```bash
cp -R skills/gf-diagnose ~/.claude/skills/gf-diagnose
cp -R skills/gf-activation ~/.claude/skills/gf-activation
```

They're now available in any Claude Code session — invoke explicitly with `/gf-diagnose`
or `/gf-activation`, or just describe the task and Claude will trigger them.

*(To use in a claude.ai Project instead: create a Project, paste the body of a `SKILL.md`
as custom instructions, and upload that skill's bundled `knowledge/` or `corpus/` files as
Project knowledge.)*

## Try it in 30 seconds

**Diagnose** — paste the sample funnel and ask to diagnose it:

```bash
cat examples/sample-weekly-funnel.csv
```

Then in Claude: *"Diagnose this funnel"* (paste the CSV). You should get a plain-language
read that flags the data-quality issues first, surfaces the sustained drop as a soft
candidate, and cites cards by id — not a confident verdict.

**Activation** — ask: *"Lots of users sign up but few ever reach first value. How do I fix
our onboarding?"* You should get a scoped answer that first pins down your "aha" moment and
checks it's actually an activation problem, then cited recommendations with honesty caveats.

## What's inside

```
skills/
  gf-diagnose/
    SKILL.md
    knowledge/        # cited knowledge cards (judgment, benchmarks, methods, principles)
    spec/             # metric spec + PLG-SaaS overlay (canonical metric ids)
    HARD-RULES.md
  gf-activation/
    SKILL.md
    corpus/           # 29 cited activation units (+ INDEX, SOURCES)
    reference/        # FRAMEWORK, HARD-RULES, GUARDRAILS (the trust tiers)
examples/
  sample-weekly-funnel.csv
```

Every knowledge card and corpus unit carries its own `provenance` and `sources` — this is
**public, cited evidence**, not model memory.

## License

MIT — see [`LICENSE`](LICENSE). Use, modify, and redistribute freely; the bundled knowledge
cards and corpus units are public, cited evidence.

---
*Galangal Flow is a per-client growth-OS assembly kit. This repo is the open sampler of its
method. Full archetype overlays + certified instances are delivered per engagement.*
