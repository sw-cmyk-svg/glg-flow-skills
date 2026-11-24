# Contributing

Thanks for wanting to improve the Galangal Flow growth-specialist skills. This repo is the **public,
open-core sampler** of the method — general PLG-SaaS specialists on a public, cited corpus. The
proprietary layer (regulated archetype overlays, certified client instances, the live-data connector)
is **not** here and is out of scope for contributions.

By contributing you agree your work is released under the repo's [MIT license](LICENSE).

## The one rule that matters: grounded + cited, never asserted

Everything in this repo lives or dies by evidence discipline. A contribution that adds an unsourced
claim, or makes a skill sound more certain than its evidence, will be asked to change.

- **Every corpus unit / knowledge card carries real, public sources.** No private data, no client
  data, no paywalled-and-unquotable sources. If you can't cite it publicly, it doesn't go in.
- **Cite, don't restate.** A unit states a principle + how to apply it + a caution, and names its
  sources. Skills cite units *by id*; they never paste a source's full text.
- **Be honest about evidence strength.** Mark a claim `correlational`, `bundled`, `second-hand`, or
  `exploratory` when that's what it is. "Engaged users do X" is not "X causes retention."
- **Aggregates only.** These skills never touch user-level rows. Don't add examples, tests, or
  guidance that assume per-user data.
- **No dark patterns.** Persuasion-adjacent tactics carry an ethics caution; manipulative tactics
  (fake scarcity, manufactured loss, guilt loops) are documented as anti-patterns, never prescribed.

## Ways to contribute

### 1. Report a skill behaving wrongly
Open a **Skill behavior** issue: which skill, what you asked, what it did, and why it's wrong
(ungrounded claim, a cited id that doesn't resolve, a scope slip, a missed guardrail, a bad analysis).

### 2. Propose or fix corpus evidence
Open an **Evidence / corpus unit** issue (or a PR). A corpus unit is one Markdown file under
`skills/<skill>/corpus/units/` with YAML frontmatter and a short body:

```markdown
---
id: ret-tactic-example-unit            # kebab-case, unique; the filename matches the id
stage: retention                        # activation | retention | monetization | acquisition | referral
sub_stage: habit
business_model: plg-saas
tactic_family: habit-formation
unit_type: tactic                       # principle | tactic | design | framework | benchmark
metric: [w1_retention]                  # related metric ids from the spec
provenance: public
sources:
  - "Author / Org — Title (year). https://public-url"
verified: 2026-11-24
---
**One bold principle line — the claim in a sentence.**

How to apply. Concrete, specific action.

When it applies / When it doesn't. The enabling conditions.

Caution. One line: the risk or the honesty caveat (evidence strength, ethics).

Related. [[another-unit-id]]
```

Knowledge cards for `gf-diagnose` live under `skills/gf-diagnose/knowledge/**` and follow that
skill's existing card shape.

### 3. Request a new specialist or feature
Open a **New specialist / feature** issue. A new specialist skill needs: a `SKILL.md` (scope rails +
modes), a bundled cited `corpus/`, the shared `reference/` files, and it must pass the behavioral bar
below.

## The behavioral bar (what a good skill does)

Before a skill change is accepted it should, on a realistic prompt:
1. **Scope first** — narrow the question before prescribing.
2. **Route off-scope asks** to the right neighbour instead of answering outside its domain.
3. **Cite every recommendation** by a unit id that actually resolves to a bundled file.
4. **Carry honesty** — evidence strength + ethics cautions, no over-claiming.
5. **Hold the guardrails** — aggregates-only data boundary; refuse dark patterns.

## Testing locally

```bash
cp -R skills/* ~/.claude/skills/          # install the skills
# in a fresh Claude session: paste examples/sample-plg-funnel.csv and ask "diagnose this",
# or ask a specialist an in-scope question, an off-scope one, and a dark-pattern bait.
```

Quick grounding check — every id a skill cites should resolve to a real file:

```bash
grep -rhoE '[a-z]{2,4}-(principle|tactic|design|framework|benchmark)-[a-z0-9-]+' skills/<skill>/SKILL.md \
  | sort -u | while read id; do test -f skills/<skill>/corpus/units/$id.md || echo "MISSING: $id"; done
```

## Pull requests

- Keep PRs small and focused (one unit, one fix, one specialist).
- Include the **public source(s)** for any new claim, and state the **evidence strength**.
- Don't add secrets, private corpus, or anything from a client.
- Update the relevant `corpus/INDEX.md` / `corpus/SOURCES.md` when you add a unit.

Questions? Open an issue — thanks for keeping it grounded. 🌱
