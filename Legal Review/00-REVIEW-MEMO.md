# Calmlyte Legal Pages — Review Memo for Attorney Review

**Prepared for:** Emma (and the reviewing attorney)
**Re:** Four legal pages — **US-only v1**
**Status:** Draft for attorney review — not legal advice, not for publication until counsel signs off.

---

## Scope decision (important)

v1 is **US-only.** An earlier pass drafted these for international sale (US + EU/EEA + UK + Canada + Australia/NZ); that was reversed as out of scope for launch. International is a materially larger legal build (GDPR/UK-GDPR, representatives, EU withdrawal function, foreign consumer law, product-safety/CE marking, VAT/GST) and is a separate future project. **The full international drafts are preserved in `_international-vNext-archive/`** and can be picked up the day Calmlyte decides to sell abroad — do not rely on them for a US launch, and do not sell/ship outside the US on the current documents.

## How to read these

- **Every section is written in final-style language.**
- **Business decisions are resolved and marked `[DECISION: ...]`** (from the answered questionnaire).
- **Company facts only Calmlyte knows remain `[CONFIRM: ...]`** — entity, domain, inbox, addresses, governing state, carrier, exactly what Stripe captures. These are filled from reality by Calmlyte, not guessed. The Privacy Policy top block consolidates them.
- Facts already established in our work are filled in: Stripe is the processor (hosted Payment Links); the static build runs no analytics, pixel, account system, or first-party cookies; GitHub Pages exposes no server logs to the owner; prices as listed; product photos are AI placeholders (an open blocker).

## The launch-blockers, ranked (US-only)

1. **Health claims / medical-device line — the dominant risk, and it's counsel's call.** Under the FDA general-wellness policy, a light-therapy device becomes a regulated medical device the instant it carries a therapeutic claim (pain, acne, wound healing, depression, sleep, etc.). Classification is driven by **claims, not hardware.** Every efficacy statement site-wide must be scrubbed to general-wellness language and confirmed against FTC substantiation rules. **Nothing goes live before this closes.** (Terms §2.)
2. **The "Pending clinical and legal review" spec note** must be gone from the **live** site before checkout is enabled — confirm and mark complete. (Terms §2.)
3. **Product photography** — AI placeholders must be replaced with real photos before sale; shipping something materially different from what's pictured is its own liability. (Terms §2.)
4. **Product safety warnings** — counsel + product to finalize warnings for a light-emitting device (eye exposure, photosensitivity, seizure risk, pregnancy, photosensitizing meds), placed with the product and in-box. US-relevant and real regardless of geography. (Terms §9.)
5. **US sales tax setup** — configure Stripe Tax by economic nexus, confirmed with the accountant, or the tax language in Terms §3 isn't accurate.

## Business decisions applied (from the answered questionnaire)

| Item | Decision |
|---|---|
| Return window | 30 days from delivery |
| Return condition | Unused/like-new, original packaging |
| Hygiene / final sale | Opened Mask final sale; same rule extended to Belt (skin) and Handheld (surface contact), unless defective |
| Restocking fee | None |
| Who pays return shipping | Customer for change of mind; Calmlyte for defective/incorrect/damaged |
| Refund timing | Within 5 business days of inspection |
| Exchanges | Return-and-reorder, no formal exchanges |
| Warranty | 1-year limited (repair/replace/refund at our option); implied warranties not fully disclaimed — **attorney drafts final clause** |
| Order acceptance | On dispatch/confirmation, not at click |
| Arbitration | **Included** — binding individual arbitration + class-action waiver, small-claims carve-out, 30-day opt-out (Terms §10; attorney finalizes wording) |
| Marketing email/SMS | None at launch (keeps CAN-SPAM/TCPA out of scope) |
| Data retention | Order records 7 yrs (accountant to confirm) / support 24 mo |
| Currency | USD, charged in USD |
| Shipping | Free flat-rate US |
| Damaged / lost windows | Damage within 7 days (photos); non-delivery within 30 days; Calmlyte covers cost |
| Address-error reshipment | Customer pays if their error; Calmlyte pays if ours |
| Checkout agreement | Checkbox at checkout (Stripe supports it) |

## Facts — mostly resolved

Applied: entity **NSH Operations LLC** · mailing/return address **PO Box 15191, Pittsburgh, PA** · governing law **Delaware** · Stripe only processor (captures name/address/email/phone) · no analytics/cookies/accounts · service providers Stripe + UPS/FedEx, no other recipients · prices confirmed · made-to-order, delivered in 10–14 business days · free US shipping, all air, all 50 states · tracking via Stripe · checkout checkbox enabled · **arbitration + class-action waiver included** (attorney to finalize wording).

**Still open (3):** final **domain**, monitored **inbox**, and a **street/receiving address for large-item returns** (a PO box can't accept a Panel Pro).

## Items requiring counsel/accountant (owners + dates are theirs)

- **Counsel:** health-claims determination (blocker #1); final drafting of warranty (Terms §7), limitation of liability (§8), safety disclaimers (§9), and the arbitration decision (§10); confirmation the checkout-agreement mechanism is enforceable.
- **Accountant:** US sales-tax setup via Stripe Tax by nexus; confirm the order-record retention period.

## Consistency check — verified (US-only)

Return window, who-pays-return-shipping, defective-item handling, and refund timing are aligned across the Terms of Sale, Shipping Policy, and Return & Refund Policy. **Re-verify all three if any `[DECISION]` value changes** — a contradiction between them is the most common and most exploitable defect in DTC legal pages.

---

*I am not a lawyer and this is not legal advice. These drafts make the reviewing attorney's job faster and surface every open decision explicitly; they are not to be published as-is.*
