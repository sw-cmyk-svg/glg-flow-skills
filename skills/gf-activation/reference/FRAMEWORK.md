# Specialist framework (fillable) v0.1

> **Extracted from the Activation instance** — the first proof (D-04: build one concretely, then
> extract). To add a domain specialist, copy this shape into `copilot/specialists/<stage>/` and fill
> the per-part blanks. **Reference instance:** `copilot/specialists/activation/` — read it as the
> worked example for every part. Don't template ahead of a second instance; this v0.1 is extracted
> from one, so expect it to firm up when Retention fills it.

## What a specialist is

A **domain-vertical specialist** owns one stage of the growth journey (activation, retention,
monetization, acquisition, referral). It is **corpus-grounded** and kept **on scope** by its
playbook's narrowing questions. It **uses** the cross-cutting **method** specialists
(Diagnose / Validate / Report) and never redefines them: it brings the *domain knowledge + scoping
rails*, they bring the *procedure*. Its job is to be **easier to get a useful, on-scope answer from
than a non-expert prompting a blank chat** — not to out-know a chatbot.

## The files (the anatomy as a fillable checklist)

Each `copilot/specialists/<stage>/` directory holds:

1. **`CHARTER.md`** — decisions owned, what it does *not* do, and the overlap/seam rules with
   neighbours so routing is unambiguous. **Fill:** the stage; the metrics it owns; the **upstream
   seam**, **downstream seam**, and **money seam** (who owns the shared metric, and the convention
   for grey-zone levers); the archetype note.
2. **Corpus binding → `corpus/<stage>/`** — provenance- and context-tagged units; cite ids, never
   restate (HR4). **Fill:** the stage's corpus slice and its tactic families, built by the corpus
   procedure below.
3. **`PLAYBOOK.md`** — the scoping rails: a **scope gate** (narrowing questions + route off-scope to
   the charter's neighbours), **analysis mode** (reuse `diagnose` on the stage's metric band),
   the **solution pipeline** (Research → Recommend → Design → Validate), guardrails inline, the
   **writing rule** (structure for scanning), and the output shape. **Fill:** the stage's value
   moment / core metric; its benchmark units; its **problem → tactic-family map**.
4. **`INPUT-CONTRACT.md`** — question + context + the `diagnose` aggregates-only CSVs (analysis mode,
   HR2) + corpus (retrieval-as-adapter) + metric spec. Mostly reusable; **fill** the stage specifics.
5. **`OUTPUT-CONTRACT.md`** — narrative-first; analysis mode reuses the `diagnose` findings shape;
   solution mode emits the recommendations block under "scoped guidance, not certified". Reusable
   schema; **fill** the stage's `tactic_family` enum.
6. **Tool bindings** — client connectors (MCP) + curated supplied OSS tools, both **degrade loudly**
   and never gate core function. **Fill:** which tools this stage curates (may be none at first).
7. **`ASSURANCE.md`** — analysis checkable (numerical faithfulness / HR2 / guardrails / cost,
   gateable); solution explainable-not-certified (provenance + honesty disciplines + the judged
   proof as evidence; the HR3 relaxation, bounded). Reusable; **fill** the stage's proof reference.

Plus **`PROOF-COMPARISON.md`** — the D-03 judged comparison for the stage.

## Cross-cutting rules every specialist inherits (don't re-decide these)

- **Uses the method specialists** (Diagnose / Validate / Report); reuses v1 `diagnose` (analysis) and
  `propose-experiments` (the rigorous-experiment branch of Validate). No forked procedures.
- **Archetype = corpus context filter** (`business_model` tag), not a new specialist. Regulated
  archetypes (bank/wallet, betting) carry a **compliance caution, not a ban**; dark patterns are
  never prescribed; out-of-corpus archetypes are flagged as **borrowed priors**.
- **Boundary rule:** method specialists are cross-cutting (defined once); knowledge specialists are
  vertical (per stage). Define the seams so two specialists never give conflicting answers.
- **Assurance split:** analysis checkable; solution explainable-not-certified — a recorded, bounded
  HR3 relaxation (bounded by the citation requirement, the honesty disciplines, and the judged proof).
- **Grounding + honesty:** every prescription cites a corpus unit or is labelled *exploratory,
  uncited* (HR4 / HR6-reframe). **Causal-vs-correlational honesty is mandatory** (pre/post ≠ causal;
  bundled ≠ isolated; second-hand flagged).
- **Writing:** structure for scanning (lead with a 2–3 line summary, clear sections, plain words,
  jargon defined on first use, no AI-writing tells) — **not brevity**; a longer grounded answer is
  fine when the content earns it. But: **don't narrate the grounding** ("the corpus says", "per the
  playbook") — the cited unit id is the grounding, state the point as fact; **a caution is a one-line
  caveat, not a paragraph**; and **be concrete** — the specific action over the general principle.
  - **Compliance caution, once then concrete.** On a regulated archetype (bank/wallet, betting), state
    the compliance / responsible-use caution **once, up front, clearly** — then get concrete with
    domain-specific guidance. Do **not** repeat the caveat on every recommendation; a wall of repeated
    cautions reads as formalism and buries the actual help. When the corpus is thin for that archetype
    (out-of-corpus), say so plainly and give the best concrete domain guidance you can, flagged as
    borrowed priors — don't substitute repeated cautions for substance.
  - **The narrative is the answer; any structured/JSON block is a terse machine-readable appendix.**
    Lead with and fully answer in prose — the founder should get everything they need without reading
    the block. Put the structured block **last**, keep it short, and never let it carry the value or
    repeat the narrative.
- **Design is a proposal** (spec + wireframe); the client ships. Never deploy or hand over production
  code.

## Corpus procedure (how `corpus/<stage>/` gets built)

- **Unit = authored, distilled note + citation** (GL's words; transformative/copyright-safe; never
  reproduces source text). YAML frontmatter tags (`stage, sub_stage, business_model, tactic_family,
  unit_type, metric [spec ids], provenance, sources`) + distilled body
  (principle / how-to / when-it-applies / caution).
- **Process = I draft, founder vets.** **Verification is part of drafting** — a benchmark/case-study
  figure is cited only after it's verified at source; second-hand figures are attributed to the
  proximate source and flagged.
- **Persuasion & ethics curation principle:** persuasion/behavioral tactics allowed, but every
  persuasion-adjacent unit carries a mandatory `Caution (ethics):` line; regulated archetypes get a
  compliance caution; outright dark patterns are documented only as anti-patterns.
- **Robust = all tactic families at ≥3 units**, diversified unit types, with ≥1 first-party benchmark
  source where possible. Target proof size ~20–40 units.

## How to add a specialist (the procedure)

1. **Build the corpus** `corpus/<stage>/` (SOURCES, INDEX, units) by the corpus procedure above.
2. **Write the files** in `copilot/specialists/<stage>/` from the checklist, filling each blank.
3. **Define the seams** with neighbouring stages in the charter (unambiguous routing).
4. **Run the judged proof** (the D-03 pattern: specialist vs a blank-chat control, independent Haiku
   judge on scope / grounding / usefulness) and record `PROOF-COMPARISON.md`.
5. **Build concretely first, then extend this template** — don't template ahead of the next instance.

## Reference instance

`copilot/specialists/activation/` — Activation, PLG-SaaS, the first proof. Every part above has a
worked example there, and `PROOF-COMPARISON.md` shows the D-03 result (specialist 0.87 vs blank-chat
0.82, grounding the differentiator).

---
*Specialist framework v0.1 · 2026-11-18 · extracted from the Activation instance (D-04).*
