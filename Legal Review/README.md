> **DRAFTS — not counsel-approved, not published. Do not link from the live site until reviewed and cleared by counsel.**

# Calmlyte Legal Pages — Draft for Attorney Review

**Status: completed US-only drafts, pending attorney review. Not for publication.**
**Scope: United States only** (v1). International drafts are archived in `_international-vNext-archive/` for a future phase.

## Files
- `00-REVIEW-MEMO.md` — **start here.** Scope decision, launch-blockers ranked, decisions applied, remaining unknowns, consistency check.
- `01-privacy-policy.md`
- `02-terms-of-sale.md`
- `03-shipping-policy.md`
- `04-return-refund-policy.md`
- `05-QUESTIONS-TO-ANSWER.md` — the questionnaire, pruned to the US subset, with answers recorded.
- `_international-vNext-archive/` — the full international versions, kept for when/if Calmlyte sells abroad. Do not use for a US launch.

## What these now are
Complete, final-style US-only drafts. Every section is written out; business decisions are applied and marked `[DECISION: ...]`; facts only Calmlyte knows remain `[CONFIRM: ...]`.

## What still has to happen before publishing
1. Fill the `[CONFIRM: ...]` facts (consolidated at the top of the Privacy Policy) — entity, domain, inbox, addresses, governing state, carrier, exactly what Stripe captures.
2. Counsel: close the health-claims / medical-device determination (the top blocker); finalize warranty (§7), limitation of liability (§8), safety warnings (§9), and the arbitration decision (§10) in the Terms.
3. Confirm the "Pending clinical and legal review" note is gone from the live site; replace AI product photos with real photography.
4. Accountant: US sales-tax setup (Stripe Tax by nexus) and confirm the retention period.
5. Re-run the consistency check if any `[DECISION]` value changes.

## After counsel finalizes
Convert the approved markdown into styled HTML pages matching the storefront (`/privacy`, `/terms`, `/shipping`, `/returns`). Do this last.

## Guiding principle
No invented facts. Where a real fact is needed it is a `[CONFIRM]` bracket, not a guess — a document that *looks* finished with fabricated facts is worse than an honest one, because it turns legal review into rubber-stamping.
