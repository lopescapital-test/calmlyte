# Calmlyte Legal Pages — Review Memo for Attorney Review

**Prepared for:** Emma (and the reviewing attorney)
**Re:** Completed drafts of the four legal pages, re-scoped from US-only to US + EU/EEA + UK + Canada + Australia/NZ
**Status:** Draft for attorney review — not legal advice, not for publication until counsel signs off.

---

## What changed and how to read these

The four files were honest *skeletons* — every fact left as an `[EMMA: ...]` bracket. The instruction was to **complete them** for a company selling wellness products in the US **and abroad**. I did that as far as it can responsibly go:

- **Every section is now written in final-style language,** including the international regimes that were entirely absent.
- **Business decisions have been resolved with recommended defaults**, marked `[DECISION: ...]` so you can see and change each one.
- **I did not invent company facts.** Things only Calmlyte knows — legal entity, domain, monitored inbox, mailing address, whether analytics is installed, exact SKUs/prices — remain as `[CONFIRM: ...]` placeholders, consolidated at the top of the Privacy Policy. Faking these would turn your review into rubber-stamping, which is the exact failure the original README warned against.

So the documents now *read as done*, but they are not publishable until (a) the `[CONFIRM]` facts are filled, (b) the `[DECISION]` defaults are approved or changed, and (c) counsel completes the regulatory items below. The next attorney should treat `[DECISION]` items as my recommendations to accept/reject and `[CONFIRM]` items as open facts.

## The five things that actually block launch (ranked)

1. **Health claims / medical-device line — the dominant risk, and it's now worse with international scope.** In all five jurisdictions (FDA, EU MDR, UK, Health Canada, TGA), a light-therapy device becomes a *regulated medical device the moment it carries a therapeutic claim* — classification is driven by claims, not hardware. Wellness-only language keeps Calmlyte out of device regulation; a single "treats pain/acne/depression/sleep disorder" claim pulls it in, per market, with clearance/registration and (in the EU) CE marking + clinical data. **Action:** counsel must scrub every efficacy statement site-wide against wellness-only positioning, per market, before launch. This is a go/no-go item, not a wording tweak.

2. **The "Pending clinical and legal review" spec note on the live product page cannot coexist with a live sale.** Resolve the review or take the specs down before checkout is enabled.

3. **Product-safety compliance for selling a light-emitting device abroad — a whole workstream that lives *outside* these four policies.** Selling into the EU almost certainly triggers the **EU General Product Safety Regulation (in force since 13 Dec 2024), which requires an EU-based "responsible person"** for the product, plus likely CE marking under the applicable electrical/EMC/RoHS directives even for a *non-medical* device; the UK has a parallel regime (UKCA / responsible person). This is analogous to the GDPR representative but for the physical product. **Action:** counsel + operations must scope this before EU/UK sales; it is not addressed by the policy pages and is easy to miss.

4. **Representatives and registrations must exist before you sell in each region.** These have **no revenue threshold** and take lead time:
   - **GDPR Art. 27 EU representative** and **UK GDPR representative** — required because you offer goods to those residents from outside. (Privacy Policy §12.)
   - **Quebec Law 25 privacy officer** and likely **French-language** versions of consumer-facing docs for Quebec. (Privacy Policy §13.)
   - **EU withdrawal function** — the mandatory online "withdraw from contract" button is in effect as of **19 June 2026**; it must be built and linked before EU sales. (Return Policy §11.)

5. **Tax registration and collection per market — an accountant workstream to confirm before the tax language is true.** US sales tax (Stripe Tax by economic nexus); EU VAT/IOSS (≤€150), UK VAT (≤£135), Canada GST/HST, Australia low-value-imported-goods GST (register at A$75k), NZ equivalent. The Terms and Shipping pages state the rules but the *setup* must be confirmed or the statements are inaccurate. (Terms §3, Shipping §4.)

## Recommended business decisions I applied (accept or change)

| Item | Recommended default | Where |
|---|---|---|
| Change-of-mind return window | 30 days from delivery | Return §1 |
| Return condition | Unused/like-new, original packaging | Return §2 |
| Opened Mask (skin/eye contact) | Final sale for hygiene unless defective (mirrors EU sealed-goods exception) | Return §2 |
| Restocking fee | None | Return §2 |
| Who pays return shipping | Customer for change of mind; Calmlyte for defective/incorrect/damaged & EU/UK statutory | Return §5 |
| Refund timing | 5 business days after inspection (14 days for EU/UK withdrawals) | Return §6 |
| Exchanges | Return-and-reorder, no formal exchanges | Return §7 |
| Warranty | 1-year limited, repair/replace/refund at our option; implied warranties **not** fully disclaimed | Terms §7 |
| Order acceptance | On dispatch/confirmation, not at click | Terms §4 |
| Governing law | State of the selling entity (needs entity confirmed) | Terms §10 |
| Arbitration | US customers only, with small-claims carve-out + 30-day opt-out; **excluded** for EU/UK/AU/NZ | Terms §10 |
| Marketing email | None at launch (keeps CASL/CAN-SPAM/e-privacy out of scope for now) | Privacy §3 |
| Data retention | 7 yrs order records / 24 mo support | Privacy §6 |
| Shipping cost | Free flat-rate US; charged international; duties = customer (DDU) unless VAT/GST collected at checkout | Shipping §3–4 |
| Handling time | 10–14 business days to dispatch | Shipping §2 |

## Genuine unknowns to fill (from the Privacy Policy top block)

Selling entity · final domain · monitored inbox · mailing address · whether any analytics/pixel is installed · confirmation Stripe is the only processor · exact current SKUs/prices · the real list of service providers (carrier, fulfillment/3PL) · return address.

## Consistency check (cross-document) — verified

Return window, who-pays-return-shipping, defective-item handling, and refund timing are aligned across the Terms of Sale, Shipping Policy, and Return & Refund Policy. **If any `[DECISION]` value is changed, re-verify these four across all three documents** — a contradiction between them is the most common and most exploitable defect in DTC legal pages.

## One caveat on scope

"Abroad" was set to EU/EEA + UK + Canada + Australia/NZ. If Calmlyte intends to ship to any country outside that list, do **not** rely on these documents for it — each additional market can add its own consumer-law, privacy, tax, and product-safety obligations, and the medical-device analysis must be redone market by market.

---

*I am not a lawyer and this is not legal advice. These drafts are structured to make the reviewing attorney's job faster and to surface every open decision explicitly, not to be published as-is.*

Sources consulted for the international requirements:
- [EU right of withdrawal & 2026 mandatory withdrawal function — EUR-Lex / Your Europe](https://europa.eu/youreurope/citizens/consumers/shopping/returns/index_en.htm)
- [GDPR Article 27 EU representative (no threshold)](https://gdpr-info.eu/art-27-gdpr/)
- [CASL / PIPEDA consent requirements — CRTC](https://crtc.gc.ca/eng/com500/guide.htm)
- [Australian Consumer Law consumer guarantees cannot be excluded — ACCC](https://www.accc.gov.au/consumers/buying-products-and-services/consumer-rights-and-guarantees)
- [FDA General Wellness Policy for Low Risk Devices](https://www.fda.gov/regulatory-information/search-fda-guidance-documents/general-wellness-policy-low-risk-devices)
