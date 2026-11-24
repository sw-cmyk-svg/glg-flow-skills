---
id: ret-framework-hook-model
stage: retention
sub_stage: habit
business_model: plg-saas
tactic_family: habit-formation
unit_type: framework
metric: [w4_retention, weekly_active_users]
provenance: public
sources:
  - "Nir Eyal — Hooked: How to Build Habit-Forming Products (2014). Model widely documented; see nirandfar.com, fs.blog/hooked."
---
**Framework — the Hook model: how a product builds a return habit (Eyal).**

A habit forms through a repeated four-phase loop:
1. **Trigger** — what starts the loop. **External** at first (a notification, an email), then
   **internal** (an emotion the product gets associated with, e.g. boredom → open the app).
2. **Action** — the simplest behaviour done in anticipation of a reward (scroll, search). Leans on
   Fogg: make it easy ([[ret-principle-fogg-behavior-model]]).
3. **Variable reward** — an *unpredictable* payoff (new content, a Like). The unpredictability is the
   engine ([[ret-tactic-variable-rewards-habit]]).
4. **Investment** — the user puts something in (data, content, connections) that improves the product
   and **loads the next trigger**.
Over cycles, external triggers give way to internal ones and the loop self-sustains.

**How to apply (Diagnose/Recommend).** Map the product's loop: what triggers a return, is the core
action easy, is there a *genuine* variable reward, and does use build value that pulls the user back?
The weakest link in the loop is where retention leaks.

**When it applies.** Products with a natural repeat-use frequency; much less relevant for genuinely
occasional tools (tax software).

**Caution (ethics).** Habit-forming is a double edge — Eyal himself later wrote on resisting
distraction. Build loops around **genuine value the user wants to return to**, not compulsion against
their interest. For bank/wallet and betting, habit loops around spending or wagering carry a
heightened caution advising responsible-use / responsible-gambling compliance; never engineer
compulsion. Manipulative triggers and infinite loops designed to maximise time-on-app against the
user's wellbeing are documented only as anti-patterns. Mirrors `copilot/GUARDRAILS.md`.
