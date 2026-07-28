# Big T's Bakery — Launch Checklist (custom site)

Replaces the earlier Wix build plan, which no longer applies. This tracks the hand-coded `index.html` + `images/` build.

## Done

- [x] Single-file site built (`index.html`), responsive + accessible
- [x] Order builder: cart, auto ฿175 bundle math, live total
- [x] Custom icing-colour field on Black & White cookies
- [x] Pickup / delivery toggle, weekend date, customer details
- [x] Real logo in nav, footer, favicon
- [x] Individual cookie photos cropped and placed (hero, signature cards, order menu)
- [x] Seasonal photos placed (banana, cranberry, pumpkin, apple crisp)
- [x] Mascot photo in Our Story
- [x] p5 "made to order" graphic — typo fixed, placed in How It Works
- [x] LINE ordering wired: QR in Contact + tappable "Open LINE" button (`https://lin.ee/5Dtfp3k`)

## You still need to do

- [ ] Push `index.html` + the `images/` folder to the repo (keep the folder name `images`)
- [ ] Deploy to a free host (Netlify / Cloudflare Pages / GitHub Pages) and point the friend's domain at it
- [ ] Eyeball the live page on a real phone once deployed
- [ ] Fill remaining `CONFIG` values as the friend sends them (see below)
- [ ] Add Instagram link to `CONFIG.instagramUrl`

## Waiting on the friend (drop into `CONFIG` / `MENU`)

- [ ] **PromptPay ID + QR image** → `CONFIG.promptPayId`, `CONFIG.promptPayQR` (this is the *payment* QR, separate from the LINE code)
- [ ] **Delivery area + fee**, free-over threshold → `CONFIG.deliveryArea`, `deliveryFee`, `freeDeliveryOver`
- [ ] **Pickup address** → `CONFIG.pickupAddress`
- [ ] **Friday cut-off time + weekend windows** → `CONFIG.leadTime`
- [ ] **Seasonal prices** → set a number on each item in `SEASONAL` to make it orderable (until then it shows "Price TBC")
- [ ] **Allergen line** confirmed (a sensible default is already in place)

## Notes

- Anything left as `TODO` in `CONFIG` renders as a **visible red placeholder** on the page, so nothing fake ships silently.
- The menu is a JS array near the top of the file — the friend's price/menu changes are one-line edits, not markup hunts.
- Held, not used on-page (redundant with existing sections): the p2 promo collage and p3 "why choose" infographic. Available in the PDF if wanted later.
- Phase 2, unchanged: card gateway (needs business registration), order-confirmation email, LINE Official Account, a small CMS so the friend edits the menu himself.
