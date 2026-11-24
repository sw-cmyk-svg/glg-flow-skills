# Hard rules — spec-level, non-negotiable

Every artifact in this repo, and every client instance stamped from it,
must satisfy all six. PRs that violate one are rejected regardless of merit.

1. **Survive our disappearance.** Every component must run without Galangal
   Lab after handoff. No pipelines on our infra, no credentials we hold, no
   scheduled jobs we babysit. Prefer zero-ETL native integrations; anything
   scheduled runs on client-owned infra under client-owned credentials.

2. **No identifying data crosses into the AI layer — by default, and always
   for regulated instances.** Direct identifiers — name, email, phone, address,
   payment or account number, precise location, or free text carrying any of
   them — do not reach the copilot. Connectors may touch raw data; the copilot
   sees aggregate and pseudonymized reads, not who anyone is.

   Aggregates (funnels, cohort tables, rates) remain the **default and
   preferred** form. Row-level data is permitted **only** where the analysis
   genuinely requires it — path and sequence analysis being the motivating
   case — and only **pseudonymized**: an opaque id the AI layer cannot resolve
   to a person without a key it never holds. Aggregate reads also carry a
   **minimum-cohort floor**: a cut that resolves to too few people
   (re-identifying by rarity) is suppressed, so "aggregate" is not treated as
   safe by shape alone.

   **The boundary is enforced at Galangal Flow's own data-acquisition adapter,
   not borrowed from the tool.** However the data is reached — an export, a
   warehouse view, or an analytics-tool API — the adapter exposes only approved
   aggregate (and, where justified, pseudonymized) reads and has **no code path
   to the raw / person-level surface**. This matters most for product-analytics
   tools (Mixpanel, Amplitude, PostHog, GA4), whose credentials scope at the
   project, not the endpoint, so the tool cannot deny raw on its own; GF's
   adapter is what denies it. The vendor also offering a raw export is
   irrelevant, because the adapter never calls it — the same guarantee as an
   aggregates-only warehouse view. Where the copilot **queries client data
   directly**, this boundary is a *configured control*, **verified per
   instance**, never assumed.

   **The boundary is default-on and waivable — never for a regulated
   archetype.** Every instance ships with it on. A **non-regulated** client who
   knowingly accepts raw / identifying data reaching the model may waive it, but
   only by an **explicit, recorded consent in the instance manifest** — never
   silently, and never by inferring consent from a connector that happens to
   allow raw. A regulated archetype (betting, wallet, and the like) **cannot
   waive it**: there the boundary is the product, and it stays on.

3. **No certified runtime without an eval baseline.** A runtime is Tier 1
   only after the full eval suite has been run and a baseline recorded on
   it. Everything else is Tier 2 (compiled, best-effort).

4. **Nothing is defined twice.** Metrics live once in `spec/`; knowledge
   lives once in `knowledge/` cards; playbooks cite both by ID and never
   restate them.

5. **Version the spec.** Every client instance records the metric-spec,
   playbook, and knowledge-base versions it was stamped from.

6. **No ungrounded judgment.** Every recommendation the copilot produces
   must cite a knowledge card that supports it — or be explicitly labeled
   *exploratory, ungrounded*. C-grade evidence is never presented as proven.

## Evidence grades

- **A** — replicated / meta-analytic support
- **B** — strong single study or broad industry consensus
- **C** — contested or anecdotal; must be hedged in any output

## Amendments

- **2026-07-21 — HR2 rewritten** (v1 → v2). Was: *"Aggregates only cross into
  the AI layer … no user-level rows. Ever."* The absolute privacy half is
  retained and sharpened (direct identifiers, never); the blanket ban on
  row-level data is relaxed to *pseudonymized, only where the analysis requires
  it*, to permit path/sequence analysis. The rule also now names the shift in
  **how** the boundary is enforced once the copilot queries data directly —
  from a structural guarantee to a per-instance configured control.

  This is a **widening of permission, not a change of behaviour**: everything
  built under HR2 v1 remains compliant, aggregates stay the default, and the
  adapter layer's `checkAggregatesOnly` validator is unchanged — Tier-B views
  stay aggregates-only. Only new row-level capabilities use the new latitude,
  and each must justify why aggregates are insufficient.

- **2026-11-20 — HR2 extended (v2 → v3).** Adds, without removing the v2
  privacy core: (a) the boundary is **enforced at GF's own data-acquisition
  adapter layer** — named explicitly for analytics-tool APIs (Mixpanel,
  Amplitude, PostHog, GA4), where credential scoping is project-level and cannot
  deny raw, so GF's adapter is the thing that denies it; (b) a **minimum-cohort
  floor** on aggregate reads, so low-cardinality cuts can't re-identify by
  rarity; (c) the boundary is an explicit **default-on, waivable control**.

  The one **behaviour change**: v2 stated direct identifiers reach the copilot
  *never, full stop*; v3 keeps that as the **default and the un-waivable rule
  for regulated instances**, but makes it **waivable by a non-regulated client's
  explicit, recorded consent** (instance manifest; never silent; never inferred
  from a permissive connector). Rationale: the boundary is GF's *product
  promise*, not a claim that the data is unsafe — a non-regulated client already
  free to feed their own raw data to an LLM may knowingly opt out, while the
  clients who buy the promise (regulated) keep it as a floor.

  Everything built to v2 stays compliant (default-on = v2 behaviour); the waiver
  is new latitude, exercised only by recorded opt-in and never for a regulated
  archetype. `checkAggregatesOnly` remains the enforcement point and gains the
  min-cohort check; the waiver and the regulated-archetype flag become part of
  the stamped instance manifest. See `.planning/spikes/2026-11-19-connector-
  landscape-and-boundary-map.md` for the adapter-shape reasoning.
