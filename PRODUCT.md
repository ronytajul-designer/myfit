# Product

<!-- impeccable:product-schema 1 -->

## Platform

web

## Stack

Static HTML/CSS with a small amount of vanilla JavaScript (`index.html`, assets under `assets/`). This repo is a standalone redesign of the myfitsize.com landing page. The production site is a separate Next.js codebase that isn't in this repo.

## Users

- **Primary buyer: small and mid-sized independent Shopify apparel merchants.** They find MyFit, install it from the Shopify App Store and set it up themselves, without a developer or a sales call. They're weighing a cheap app against the risk of it hurting their store's look, speed or conversion.
- **End user: the merchant's shoppers.** They're on a product page, unsure which size to buy, and answer a short quiz to get one recommended size. They never sign up for MyFit and shouldn't notice it's a third-party tool.
- **Secondary buyer: larger stores (Shopify Plus, multi-store brands).** They can book a 15-minute walkthrough. This path is secondary to self-serve install.

## Product Purpose

MyFit is a Shopify app that adds a size quiz to apparel product pages. Shoppers answer a few questions (gender, age, height, weight, fit preference) and get one recommended size matched to the merchant's own size chart. The goal is fewer size-related returns and fewer shoppers leaving because they're unsure of their size.

Success for a merchant: they install free, go live in minutes, and see quiz completions turn into purchases rather than returns.

## Positioning

A size quiz that uses the merchant's own size chart, lives inside the Shopify theme as a native block, takes on the store's own styling, and costs $4/month for unlimited use. It aims to replace the static size chart (a grid shoppers must measure themselves against) with a single answer.

## Operating Context

- Merchants evaluate it on the Shopify App Store listing and on myfitsize.com, often comparing the two.
- Setup happens in the merchant's Shopify admin:
  1. Install the app.
  2. Import a size chart (an uploaded screenshot or photo is converted into a size chart).
  3. Drag the MyFit block into place in the theme editor (for example, between Variant picker and Buy buttons).
  4. Style the button and quiz screens.
  5. Choose languages.
- Merchants review quiz completions and recommended sizes in a MyFit dashboard.
- Shoppers use the quiz mid-purchase, mostly on mobile.

## Capabilities and Constraints

Confirmed by the founder on 2026-11-04:
- **Pricing:** Free plan covers 25 quizzes a month with no credit card. Unlimited is $4/month for unlimited quizzes, with a 14-day free trial. Billed through Shopify.
- **Languages:** the quiz runs in 40+ languages, including right-to-left languages such as Arabic. The Shopify App Store listing, which shows 5 languages, is out of date and needs updating.

Observed in product screenshots (not separately confirmed):
- Garments map to body zones (upper, lower, full body), each with a starter set of measurements the merchant can adjust.
- The quiz includes at least one visual step: a body diagram for waist measurement.

Terminology:
- **size quiz:** what shoppers fill in.
- **recommended size:** the answer they get.
- **MyFit block:** what merchants place in the theme editor.
- Avoid "widget", which contradicts the "not a third-party widget" positioning.

Unconfirmed. Do not state these as fact until confirmed:
- Theme support: Online Store 2.0 only, or vintage themes too.
- What counts as one billable "quiz".
- Whether Unlimited includes extra analytics beyond the Free plan.
- How "returns prevented" is measured.
- Script weight and performance impact on the storefront.
- What shopper data is stored, where it's hosted, how long it's kept, and GDPR status.
- Whether footwear and kids' sizing are supported.
- Whether brand styling is automatic or set by the merchant, and whether the Free plan shows a "Powered by MyFit" mark.
- Company name: the footer says "MyFit Inc."; the App Store developer is "Redcircle Digital".
- Whether the sales walkthrough form needs a phone number.

The product is Shopify-only today. Don't present other commerce platforms as supported.

## Brand Commitments

- Name: **MyFit** (domain myfitsize.com). App icon: `assets/img/icon.svg`.
- Voice on the live site: direct, merchant-to-merchant, objection-first headlines ("Stop losing sales to size guesses.", "Looks like part of your store. Not a third-party widget.").

## Evidence on Hand

- Shopify App Store rating: 5.0 from 6 reviews (as captured 2026-11-04).
- Product demo recording: `assets/media/demo.mp4`.
- Product screenshots: `assets/img/slide-1.webp` to `slide-5.webp` (size chart import, merchant dashboard, quiz styling, theme placement, languages).
- Garment photography: `assets/img/apparel-*.webp` and `store-product.webp`.
- Critique and audit, 2026-11-04: `docs/critique-2026-11-04.md`. Copy changes and open facts: `docs/copy-deck.md`.

Absent. Future work must not invent these:
- Customer logos: the seven brands on the live site (nudge, LOT., JJ's House, Grey Moritz, Nuvira, VILA, Girav) are **not confirmed** as current customers. Don't label them as customers until they are.
- No testimonials, case studies or named merchant results.
- No MyFit outcome metrics (returns reduction, completion rate, conversion lift).
- The industry stats on the live site (42%, $25+, 52%) have no sources.
- No accuracy figures for recommendations.

## Product Principles

1. **Self-serve first.** Every surface should help a small merchant decide and install on their own. The sales walkthrough is a secondary path for larger stores, never the default ending.
2. **Show the price and the product, not adjectives.** The $4 price, the free tier and the real quiz in action reduce risk more than superlatives do.
3. **One source of truth.** The website, the App Store listing and in-app copy state the same facts. A contradiction found by a merchant costs more trust than any claim earns.
4. **Invisible to shoppers.** MyFit should feel like part of the merchant's store, never like a third-party tool.
5. **Earn claims with evidence.** Numbers, customer names and outcomes appear only when they're real and sourced.

## Accessibility & Inclusion

- Shoppers enter body data (age, gender, height, weight). Treat this as sensitive: privacy handling must be stated plainly once confirmed.
- The quiz serves 40+ languages, including right-to-left, so layouts and copy must survive text expansion and RTL mirroring.
- Target WCAG 2.2 AA on marketing surfaces: labelled form fields, visible focus, 4.5:1 text contrast, and 24px minimum tap targets (44px preferred on mobile).
