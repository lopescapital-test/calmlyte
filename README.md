# Calmlyte Storefront — Deploy Notes

## What this is
Production-prepped static storefront. No backend required. Payments are stubbed
(buttons show a "checkout opens soon" toast) until you paste Stripe links in.

## Structure
```
index.html          Hero storefront: intro gate + interactive mode-switcher
                    (Haven/Focus/Stillness/Dusk), rooms, family grid, learn teaser
products/           Shop index + 5 product pages (signature-panel, belt, mask,
                    handheld, panel-pro)
learn/              green-light.html (counsel-cleared spectrum article), faq.html
assets/
  forest-*.webp     4 scene backgrounds (forest-haven doubles as the intro gate)
  sig-*.webp        3 Signature Panel room shots (day / still / dusk)
  panel-<mode>.webp 4 per-mode Signature Panel scenes (hero stage + PDP use haven)
  belt/mask/handheld/panel-pro.webp  product scene shots
```
Total payload: ~1.5 MB, fully cacheable. The homepage accepts both #haven and
legacy #/haven hashes; arriving on a mode hash skips the intro gate.

## Naming
The $600 panel is the **Signature Panel** site-wide (renamed from "Small Panel",
2026-07-04). The Stripe SKU stays `small-panel` and the asset file stays
`product-small-panel.webp` — display name and URLs only. NOTE: the Legal Review
drafts still say "Small Panel"; apply the rename there via Emma/counsel during
the copy re-review (do not edit those drafts directly). The redesign also
rearranges cleared copy and adds new mode-blurb language — counsel pass required
before go-live.

## Deploy (GitHub Pages — same flow as NeuroHome)
```powershell
cd site
git init; git add .; git commit -m "Calmlyte storefront v1"
git branch -M main
git remote add origin https://github.com/<you>/calmlyte.git
git push -u origin main
# Repo Settings > Pages > Deploy from branch > main / root
```
Hash routing (`#/haven`, `#/focus`, `#/stillness`, `#/dusk`) works on any static
host — no server config needed. Deep links and back button work.

## Turning on payments later (~10 min)
1. Stripe Dashboard → Products → create the 5 SKUs → generate a Payment Link each.
2. In `index.html`, find `CHECKOUT_LINKS` at the top of the `<script>` block and
   paste each link in place of `null`. Done — buttons redirect to Stripe.

## Before you flip payments on (required)
- **Legal pages**: privacy policy, terms, and a shipping/returns policy.
  Stripe requires these and card networks will flag their absence. Do not
  generate boilerplate — have Emma or counsel produce them.
- **Spec bands** currently read "Pending clinical and legal review." Resolve
  the review and remove the note, or remove the spec bands. A live checkout
  next to that disclaimer is a liability problem.
- **Contact email**: `hello@calmlyte.com` is a placeholder in the footer and in
  the checkout toast (`CONTACT_EMAIL` in the script). Set up the real inbox.
- **Domain**: once live, uncomment the canonical tag in `<head>` and change
  `og:image` to an absolute URL so link previews work.

## What was changed from the mockup
- Extracted 30 embedded base64 images → 9 unique files, deduped, converted to
  WebP (2.1 MB → 1.34 MB), semantic filenames.
- Real hash routing with per-page titles (was display:none toggles with no URLs).
- SEO: meta description, Open Graph, Twitter card, theme-color, SVG favicon.
- All product images `loading="lazy"`; scene backgrounds hydrate on navigation.
- Buy buttons wired to `data-sku` + central `CHECKOUT_LINKS` config; graceful
  toast while links are null.
- Removed ~2 KB of dead CSS from an earlier mockup iteration (.intro/.moment/
  .closer/.buycard/.modeband blocks, one of which referenced a 300 KB image).
- Design, copy, and layout untouched.
