---
id: ref-tactic-reduce-invite-friction
stage: referral
sub_stage: invite-mechanics
business_model: plg-saas
tactic_family: invite-mechanics
unit_type: tactic
metric: [new_signups]
provenance: public
sources:
  - "Established referral/CRO practice — every tap and field between the intent to invite and a sent invite loses invites; offer the channels the user already uses; pre-fill where honest. Lowering invite friction raises the invites-sent term of k-factor."
---
**Tactic — remove taps and fields between "I'll share this" and a sent invite; each one loses invitations.**

The invites-sent half of k-factor is a funnel of its own, and it leaks at every step: finding the share
option, choosing a channel, composing a message, confirming. Cut each step. Give a **one-tap shareable
link** as the default (no login wall for the invitee to see what they're joining), offer the **channels the
user already uses** (native share sheet on mobile, link + email + the one or two social/chat apps that fit
your audience) rather than forcing one, and **pre-fill** a sensible default message the user can edit.
Removing a single required step (a mandatory custom message, an extra confirmation) often lifts invites
sent more than any reward increase.

**How to apply.** Map the invite flow as a funnel and count the taps from intent to sent. Default to a copy-
able link + native share; add email/other channels as options, not gates. Pre-fill the message and the
reward context ("you both get X"). Make the invitee's landing honest and low-friction — they should see the
value and who invited them before being asked to sign up. Measure invites-sent and acceptance separately so
you know which half to fix.

**When it applies.** Building or improving an invite flow; a program where users *start* to share but few
invites actually get sent, or sent invites don't convert.

**Caution (ethics):** low friction must not become **coercion or spam** — never auto-send on a user's
behalf, never pre-check "invite all my contacts," never import an address book without explicit opt-in (see
[[ref-tactic-invite-anti-patterns]]). Pre-filled text must be truthful, not a fake personal endorsement the
user didn't write. Pairs with [[ref-principle-contextual-share-surfaces]] (where the prompt lives) and
[[ref-framework-viral-loop-k-factor]] (friction sits in the invites-sent term).
