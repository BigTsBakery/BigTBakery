# Big T's Bakery — Wix Build Plan (v1)

Made-to-order cookie shop. Real online ordering, pickup + local delivery. Built on Wix Stores.

---

## 1. Scope for v1 (what we ship first)

**In:** menu with photos, online ordering, custom icing-colour requests, pickup + local delivery scheduling, the story, contact + socials, payments.

**Phase 2 (deliberately not now):** catering request form, gift-box builder, seasonal collections as a separate shop, pop-up / mobile-storefront pages, Facebook/TikTok integration.

Cutting Phase 2 is the point. A tight 6-page site that takes orders beats a sprawling one that doesn't launch.

---

## 2. Site map

Six pages. Don't add more for v1.

- **Home** — hero, signature cookies, how-it-works, trust badges, footer
- **Menu / Shop** — the Wix Store (cookies + seasonal)
- **Customise** — how the made-to-order + icing-colour flow works
- **Our Story** — the young-entrepreneurs angle
- **Seasonal** — rotating specials (banana bread, cranberry bread, pumpkin pie, apple crisp)
- **Contact & FAQ** — hours, area, lead time, socials, LINE

---

## 3. Brand kit (you already have the assets — just load them)

They have a finished logo, product photos, and a brand direction, so this is fast.

Pull the palette straight from the logo: warm brown, cream/tan, gold, red heart accent. Set these as your Wix site colours once so every section inherits them. Match the logo's bold vintage display face for headings and a script for taglines only (never body text — the "Gary Provost rhythm" you like lives in readable body copy, not decorative fonts).

Reuse their existing lines — they're good:
- *"Big Cookies. Big Smiles. Big T's!"*
- *"Fresh. Made to Order. Made with Love."*
- *"T-T-T-T'Soot!"* (the Thai pun is a local-charm asset — keep it visible)

---

## 4. The Store — products, pricing, and the one tricky build

### Products & prices (from the questionnaire)

| Product | Price |
|---|---|
| Small cookie pack | 3 for ฿100 |
| Large cookie | ฿60 each, or 3 for ฿175 |
| Signature: Chocolate Chip | (set as large-cookie price) |
| Signature: Birthday Cake | (set as large-cookie price) |
| Signature: Black & White (customisable) | (set as large-cookie price) |
| Seasonal: banana bread, cranberry bread, pumpkin pie, apple crisp | TBC — need prices |

Use a **"3 for" price via a quantity-based pricing rule or a distinct "3-pack" product**, not a coupon — coupons complicate reporting.

### The custom icing colour — the only non-obvious part

The Black & White cookie needs custom colours. In Wix Stores this is a **Product Option**, and you have two choices:

- **Dropdown option** ("Icing Colours") with preset choices — birthday, sports-team colours, holiday, etc. Clean, but every combo you list becomes a variant.
- **Custom text field** ("Tell us your colours") — a free-text box the customer fills in. No variants, no inventory headache, maximum flexibility.

**Recommendation:** custom text field as the primary input, plus a short dropdown of 3–4 popular presets for people who don't want to think. Made-to-order means you're not tracking colour inventory anyway, so free text is the right fit.

### Made-to-order lead time

Everything is baked to order, so the store must stop customers booking a same-hour pickup. Set a **minimum prep/lead time** and only offer pickup/delivery windows that respect it. Verify the current Wix Stores fulfilment settings still let you enforce a lead time the way you want before you build the checkout around it — Wix changes this UI periodically, and this is the setting most likely to trip you up.

---

## 5. Ordering & fulfilment

- **Pickup + local delivery** only for v1 (matches the home-bakery model).
- Define the **delivery radius and fee** — a flat local fee is simplest. Need this from the friend.
- Set **pickup windows** and a **minimum order** if you want one.
- Every order needs a **required date field** for the pickup/delivery day, respecting the lead time above.

---

## 6. Payments — manual PromptPay first, card gateway later

**Decision for v1: launch on manual PromptPay / bank transfer. No card gateway yet.**

Why: a payment gateway isn't a monthly cost — it's a per-sale % fee. At ฿60–175 order sizes, and with a business that may not be registered yet, a card gateway is the wrong first step. Manual PromptPay is how Thai customers already pay, costs effectively nothing per transaction, and needs no gateway onboarding.

### v1 — manual methods (set up now)

- **PromptPay QR / bank transfer** as a Wix "manual payment" method: customer transfers, sends proof, you confirm the order. Zero processing fee.
- **Cash on pickup** — enable it too; it's natural for local pickup.
- Add a clear "how to pay" note at checkout and in the confirmation email (PromptPay number / QR + how to send proof — LINE is the easy channel for this).

Trade-off to accept: manual means someone confirms each payment by hand. Fine at launch volume; revisit when order count makes it annoying.

### Phase 2 — card gateway (only when it's justified)

Add a Thai gateway **if** volume grows and the bakery becomes a registered business. Rough Thai rates (approximate, verify, +7% VAT): **cards ~2.5–3.65%**, **PromptPay-via-gateway ~0.8–1.65%**. Most non-bank gateways (Omise/Opn, Xendit, 2C2P) charge no setup or monthly fee.

Two things to check **before** committing to any gateway:
1. **Wix compatibility** — confirm the gateway actually integrates with Wix Stores in Thailand (many advertise WooCommerce/Shopify plugins, not Wix). Verify against Wix's accepted-providers list.
2. **Onboarding** — gateways generally require business registration and Bank of Thailand compliance, plus business banking. That's the real hurdle, not the fee.

### Either way

Whatever method is live, it must attach to the **friend's account** (the business owner) — ties back to the ownership decision in the intro.

---

## 7. Page-by-page content (drafted in their voice)

Starter copy pulled from the questionnaire. Edit freely.

**Home — hero**
> **Big Cookies. Big Smiles. Big T's!**
> Fresh, made-to-order cookies and desserts, baked with care and made just for you. Support local. Support young entrepreneurs.
> [Order Now]

**Home — why us** (reuse their icon row)
Gourmet cookies · Fresh ingredients · Made with love · Made to order · Support local young business · Pickup & delivery

**Our Story**
> Big T's Bakery started with a simple idea: make incredible desserts while building something of our own. As a collective of young entrepreneurs, we use baking to grow real business skills, express our creativity, and connect with our community. Every cookie is made fresh to order — and every purchase helps a local, independent business built on quality, creativity, and community.

**Customise — how it works**
> 1. Choose your goodies. 2. Customise (if available). 3. Pick your time and place.
> Our Black & White cookies come your way — tell us your colours for birthdays, holidays, school events, sports teams, or any occasion, and we'll make it yours.

**Seasonal**
> Made for every season. Limited-time favourites — banana bread, cranberry bread, pumpkin pie, apple crisp — baked fresh when they're in season. Follow us so you don't miss a drop.

**Contact & FAQ**
Hours, service area, order lead time, socials, LINE. (FAQ answers the predictable ones: How far ahead do I order? Do you deliver to me? Can I customise colours? Payment methods?)

---

## 8. SEO, local & social

- **Google Business Profile** — set this up early. For a local bakery, "cookies near me" traffic matters more than on-page SEO.
- **Instagram feed embed** on Home (they're active there).
- **LINE** — add a LINE contact/official-account button. In Thailand this is often where the actual ordering conversation happens; don't bury it.
- Basic on-page SEO: real page titles, alt text on the product photos they already have, a location keyword.
- FB / TikTok links: leave placeholders, wire up in Phase 2.

---

## 9. Pre-launch checklist

Your `project_workflow.md` is a full-stack governance doc — most of its 13 phases (RLS, auth, hosting, monitoring, deploy pipeline) are things **Wix handles for you**. Here's the trimmed version that actually applies:

- [ ] All products have photos, prices, and descriptions
- [ ] Custom icing-colour field works end-to-end (place a test order)
- [ ] Lead time enforced — can't book pickup inside the prep window
- [ ] PromptPay/bank-transfer manual payment set up and tested with a real small transfer; cash-on-pickup enabled
- [ ] Pickup windows + delivery area/fee correct
- [ ] Order confirmation email fires to customer **and** to the bakery
- [ ] Mobile layout checked (most Thai traffic is mobile)
- [ ] Contact info, hours, LINE all correct
- [ ] Custom domain connected, HTTPS on (Wix default)
- [ ] Google Business Profile live
- [ ] Test the whole flow on a phone as a real customer would

---

## 10. Phase 2 (after launch)

Card payment gateway (when volume + business registration justify it, see §6) · catering request form · gift-box builder · seasonal collections · pop-up / market / mobile-storefront pages · FB + TikTok · reviews/testimonials.

---

## 11. Open items — need answers before checkout goes live

1. **Whose Wix account** does this live on — yours or the friend's? (Payments attach to the owner.)
2. **PromptPay number / QR** for the business, so the manual payment method + checkout note can be set up (see §6).
3. **Dietary info** — the questionnaire left vegan/GF/halal/allergens blank. At minimum add an allergen line.
4. **Seasonal item prices.**
5. **Delivery area + fee**, and **operating/pickup windows**.
6. **Domain** — do they own one, or need to buy?
