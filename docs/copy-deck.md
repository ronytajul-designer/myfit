# MyFit landing page: copy deck (clarify pass)

Source: https://www.myfitsize.com/ as captured 2026-11-04. Audience: Shopify apparel merchants deciding whether to install. Mode: Persuade.

Legend:
- **[VERIFY]** marks a factual claim I can't confirm from the page. Pick the true version before shipping.
- **[DATA]** marks a placeholder that needs a real number from you.
- Pricing figures come from the Shopify App Store listing as captured on 2026-11-04.

---

## 0. Terminology (apply everywhere)

| Concept | Use | Stop using | Why |
|---|---|---|---|
| What shoppers fill in | **size quiz** | "visual quiz", "fit guide", "Guided Quiz" | One name per concept. "Visual" is disputed (see 2.2). |
| What they get | **recommended size** | "one exact size", "the right size" | "Exact" promises a guarantee the product can't make. |
| What merchants install | **MyFit block** | "widget", "MyFit Button", "Widgets" | The page says "Not a third-party widget" and then calls it a widget 4 times. |
| Billing unit | **quiz** (one shopper getting a recommendation) [VERIFY definition] | "quiz requests", "quiz volume" | Merchants can't predict their bill from "requests". |
| CTA verb | **Install free** | "Install Free", "Start free trial" | Sentence case everywhere. One verb per destination. |

Rule: each label names where it goes. App Store links say "Install". Links to the demo form say "Book a walkthrough". Scroll anchors say what the visitor will see when they land.

---

## 1. Nav

| Current | Proposed | Why |
|---|---|---|
| Features · FAQ · Help Center · Contact us | How it works · Pricing · FAQ · Help center | Adds Pricing, the most likely merchant question. "Contact us" moves to the footer. Sentence case matches the rest. |
| Install Free | Install free | Case consistency. |

---

## 2. Hero

**2.1 H1**: keep "Stop losing sales to size guesses." It's specific and speaks to merchants.

**2.2 Subhead**
- Current: "A 60-second visual quiz gives every shopper one exact size before checkout."
- Proposed: "Shoppers answer a few quick questions on your product page and get a recommended size from your own size chart. It takes under a minute."
- Why: "exact" overpromises, and "visual" doesn't describe an age/height/weight form. "From your own size chart" answers the merchant's first doubt ("whose sizes?").
- [VERIFY] If the quiz really has visual steps (body-shape pickers), keep "visual" and show one of those steps in the hero mockup.

**2.3 Proof row under the CTA**
- Current: "Live in 2 minutes · No developer needed · Works with any theme"
- Proposed: "Free for 25 quizzes a month · Unlimited $4/month · No developer needed"
- Why: price is the strongest risk reducer you have, and right now it's hidden. "Live in 2 minutes" is already said in the FAQ.
- [VERIFY] "Works with any theme": Shopify theme app blocks only work on Online Store 2.0 themes. If you don't support vintage themes, the honest version is "Works with any Online Store 2.0 theme". Put it in the FAQ (see 8.7).

**2.4 Secondary CTA**
- Current: "See what you get" (goes to #features)
- Proposed: "See how setup works"
- Why: it lands on the setup carousel, so the label should say what's there.

**2.5 Demo mockup caption**
- Current: "HOVER TO WATCH DEMO" / "TAP TO WATCH DEMO"
- Proposed: a visible caption above the mockup, "What your shoppers see", plus a play control labelled "Play shopper demo".
- Why: the mockup's "Find your size / Your age" reads as consumer-facing. The caption tells a merchant it's their shopper's view. "Hover" describes the gesture, not the outcome, and doesn't exist on touch.
- Accessibility: name the control `aria-label="Play shopper demo"`. Set `aria-hidden="true"` on the mockup's inner form text so screen readers skip the fake fields ("Your age", "Male").

**2.6 Trust strip**
- Current: "TRUSTED BY APPAREL BRANDS"
- Proposed: "Rated 5.0 on the Shopify App Store (6 reviews)", then "Used by stores like" + logos.
- [VERIFY] Only keep "Used by" if every logo is a paying or active customer.
- Trade-off: a perfect 5.0 from few reviews earns less trust than a 4.x from many ([Spiegel Research Center](https://spiegel.medill.northwestern.edu/how-online-reviews-influence-sales/) found purchase likelihood peaks around 4.0 to 4.7). Show the count anyway; hiding it reads worse once a merchant clicks through. Confidence: medium.

---

## 3. Problem section

**3.1 H2**
- Current: "The size problem is the single biggest tax on apparel ecommerce."
- Proposed: "Size guesses cost you twice: once at checkout, again at returns."
- Why: "single biggest" is an unsourced superlative. The rewrite sets up both stats below (hesitation and returns) without claiming a ranking.

**3.2 CTAs**
- Current: "Start free trial" (goes to the demo form) + "View widget demo" (goes to the carousel)
- Proposed: one CTA, "Install free", linking to the App Store.
- Why: "Start free trial" leads to a sales form, which breaks [information scent](https://www.nngroup.com/articles/information-scent/). Two CTAs pointing to two wrong places cost more than one right one.

**3.3 Stats** (fix the grammar and add sources, or cut the band)

| Current | Proposed |
|---|---|
| 42% / Size-related returns / "Of all online apparel returns happen because of size and fit issues" | **42%** of online apparel returns are due to size or fit. *Source: [DATA: publisher, year]* |
| $25+ / Cost per return / "Average cost to process a single size-related return" | **$25+** to process one size-related return. *Source: [DATA]* |
| 52% / Purchase hesitation / "Of shoppers hesitate or abandon when unsure about size" | **52%** of shoppers hesitate or leave when they're unsure of their size. *Source: [DATA]* |

The current lines start with "Of", which only works if the visitor reads the number as part of the sentence. If you can't cite a source, remove the band: industry numbers with no source build no trust in MyFit. The better version replaces them with your own figure ("Stores using MyFit see [DATA]% fewer size returns").

---

## 4. Setup carousel

- H2 "Set it up once. It runs on every product page after that.": keep.
- "THEME PLACEMENT / Drag the button exactly where it belongs." Change to "Drag the MyFit block exactly where it belongs."
- Body "MyFit's button works as a native block in the Shopify theme editor. Put it wherever your layout needs it, no code needed." Change to "MyFit is a native block in the Shopify theme editor. Drop it wherever your layout needs it. No code."
- **Languages slide** [VERIFY]:
  - The slide says "40+ languages" and "Your shopper in Dubai reads it right-to-left". The App Store lists 5 languages (English, Dutch, French, German, Spanish), and none of them is right-to-left.
  - If the App Store is right: "Your shopper in Berlin reads it in German. Your shopper in Madrid reads it in Spanish." Slide title: "5 languages".
  - If the site is right: update the App Store listing the same day.
- Dot button names: change "Go to 40+ languages" to match the verified slide title.

---

## 5. Brand-match band

| Current | Proposed | Why |
|---|---|---|
| "Colors, fonts, button styles, everything matches your store." | "Colors, fonts and button styles match your store." | Fixes the run-on sentence and keeps the meaning. [VERIFY] whether matching is automatic or set by the merchant. If it's set by the merchant: "Set the colors, fonts and button style once. It matches everywhere." |
| "Your shoppers never know it's MyFit." | Keep. | [VERIFY] There must be no "Powered by MyFit" mark on the Free plan. If there is one, write "Your shoppers never see a MyFit logo on Unlimited." |
| Text link "Install Free on Shopify" | "Install free on Shopify", rendered as a button | It's the only CTA in the middle of the page and currently looks like a footnote. |

---

## 6. Garment coverage

- H2 "If you sell it as apparel, MyFit can size it.": keep.
- Body
  - Current: "Each body zone: upper, lower, or full body, comes with a recommended set of measurements. You decide which measurements matter, not a fixed template."
  - Proposed: "Every garment maps to a body zone (upper, lower or full body) with a starter set of measurements. You choose which ones count."
  - Why: the colon-and-comma structure reads as a broken list.

---

## 7. Feature grid

**H2**
- Current: "Everything you need to reduce returns and grow conversion."
- Proposed: "What runs on every product page."
- Why: the current heading is a template line any SaaS page could use. The rewrite also removes the forced line break that leaves "reduce" alone on its own line on mobile.

**Cards** (drop the metric chips unless each one shows a real number)

| Card | Current | Proposed | Note |
|---|---|---|---|
| Size Finder | "Recommends the right size for every shopper, based on body shape and fit preference." | **Size recommendations**: "One recommended size per shopper, based on height, weight, age and fit preference." | The quiz never asks about body shape. Match what it actually asks. |
| Guided Quiz | "A short, visual quiz shoppers actually finish — no measuring tape, no guesswork." | **Size quiz**: "A short quiz shoppers finish without a measuring tape." | "Actually finish" needs a completion rate: [DATA]%. If you have it, say it: "[DATA]% of shoppers who start it finish it." |
| Widgets | "Buttons and quiz screens that match your brand — colors, fonts, and layout." | **Brand styling**: "The button and quiz screens use your colors, fonts and layout." | Removes "widget" (see section 0). |
| Real-time Insights | "See quiz completions, recommended sizes, and returns prevented in one view." | **Dashboard**: "See quiz completions and recommended sizes for every product." | [VERIFY] how "returns prevented" is measured. It's a counterfactual. If you can't explain the method, drop it. |
| Easy Widget Setup | "Install and go live in minutes — no code, no developer, no theme edits." | **Setup in minutes**: "Install, drag the block into place, go live. No code." | "No theme edits" contradicts "drag the block in the theme editor". |
| Multi Languages | "Serve international shoppers with built-in multi-language quiz support." | **Your shoppers' language**: "The quiz runs in [5] languages: English, Dutch, French, German and Spanish." | A real number and list beat "multi-language". [VERIFY] the count. |

---

## 8. FAQ

**8.1 Is MyFit free to use?**
- Current: "Yes. MyFit has a free plan with no credit card required — install it, build your quiz, and go live at no cost. Paid plans unlock higher quiz volume and advanced analytics as you grow."
- Proposed: "Yes. The Free plan covers 25 quizzes a month with no credit card. Unlimited is $4/month for unlimited quizzes, with a 14-day free trial. You can switch or uninstall anytime."
- [VERIFY] whether Unlimited includes "advanced analytics". If it does, add it to the answer.

**8.2 Will MyFit slow down my store?**
- Current: "MyFit installs as a native block in your Shopify theme rather than as custom code injected into your template, so it behaves like any other section of your theme and there is nothing for you to maintain."
- Proposed: "No. MyFit adds about [DATA] KB, only on product pages that use the block, and it loads after your page content. Shoppers see your page at the same speed."
- Why: the current answer never says yes or no. Merchants read that as "yes, it does".

**8.3 Do I need a developer?**
- Current: "...you are live — usually within a couple of minutes. No code and no theme edits."
- Proposed: "No. Install from the Shopify App Store, drag the MyFit block into place in the theme editor, and you're live, usually in a couple of minutes. No code."

**8.4 How is this different from a static size chart?**
- Current: "...MyFit asks a few short questions — age, height, weight, fit preference — and returns one recommended size for that specific product."
- Proposed: "A size chart hands shoppers a grid and asks them to measure themselves. MyFit asks a few short questions (gender, age, height, weight and fit preference) and gives one recommended size for that product."
- Why: adds gender, which the quiz actually asks.

**8.5 Does MyFit work for all types of apparel?**
- Current: "Yes — tops, bottoms, dresses, outerwear, swimwear and more..."
- Proposed: "Yes for clothing: tops, bottoms, dresses, outerwear, swimwear and more. Each garment maps to a body zone, and you choose the measurements that matter. [VERIFY] Footwear and kids' sizing aren't supported yet."

**8.6 New: What shopper data does MyFit store?**
- Proposed: "[DATA: what's stored, where it's hosted, how long it's kept, whether it's linked to the customer.] MyFit is GDPR compliant [VERIFY]. Shoppers can [DATA: how they delete their data]."
- Why: shoppers type in their age, gender, height and weight. EU merchants will ask this before installing. Answering it on the page removes a reason to book a call.

**8.7 New: Does it work with my theme?**
- Proposed: "MyFit works with any Online Store 2.0 theme, including Dawn and all free Shopify themes. [VERIFY: vintage theme support.]"

**8.8 New: How accurate are the recommendations?**
- Proposed: "[DATA: method and evidence, e.g. 'Recommendations come from your size chart plus [model]. Stores see [X]% fewer size returns.'] If you can't support a number yet, explain the method and skip the claim."

**Link under the FAQ**
- Current: "Still have a question? Book a demo"
- Proposed: "Still have a question? Ask us" (goes to /contact)
- Why: a question doesn't need a 15-minute sales call.

---

## 9. Demo form

**9.1 H2**: keep "Book a free, 15-minute demo with a specialist", or, if self-serve is the main path, use "Running a larger store? Book a 15-minute walkthrough."

**9.2 Intro**: keep "See MyFit running on your own products before you install anything. We'll walk through your size charts and show you what the quiz would recommend."

**9.3 Field labels** (visible `<label>` elements, not placeholders; mark optional fields instead of marking required ones with asterisks)

| Current | Proposed label | Example / helper |
|---|---|---|
| placeholder only | First name | |
| placeholder only | Last name | |
| placeholder only | Work email | Example: name@yourstore.com |
| "Country" (unlabelled select, defaults to Netherlands) | Country | Default to the visitor's country, or "Select a country". Never pre-select Netherlands for everyone. |
| "Phone number" + "+31" | Phone number (optional) | [VERIFY] whether sales needs it. If it isn't required, mark it optional. |
| "What commerce platform do you use?*" with WooCommerce, Magento, BigCommerce | Which Shopify plan are you on? | Options: Shopify · Shopify Plus · Not on Shopify yet. Add helper text: "MyFit currently works on Shopify only." |
| "How did you hear about MyFit?*" | How did you hear about us? (optional) | Attribution data isn't worth a lost lead. |
| (missing) | Store URL | It's what sales actually needs to prepare the demo. Add it if you remove phone. |

**9.4 Consent line**
- Current: "MyFit uses the details you share here to contact you about the product. You can unsubscribe at any time — see our Privacy Policy for how we handle your data."
- Proposed: "We use these details to contact you about MyFit. You can unsubscribe anytime. Our Privacy Policy explains how we handle your data."
- This keeps the same legal meaning. Have whoever owns the policy sign off on it anyway. Render it at 13px or larger.

**9.5 Button**: keep "Book my demo".

**9.6 States** (I couldn't see these without submitting the form. Write them if they don't exist.)
- Missing field: "Enter your first name."
- Invalid email: "Enter an email like name@yourstore.com."
- Send failed: "We couldn't send your request. Check your connection and try again, or email [DATA: address]." The form keeps everything the visitor typed.
- Success: "Thanks, [first name]. We'll email [email] within [DATA: 1 business day] to pick a time."

---

## 10. Footer

| Current | Proposed | Why |
|---|---|---|
| "How It Works" + "Features" (both go to #features) | "How it works" only | Two labels for one place. |
| "Pricing" (goes to /help#billing, which has no prices) | "Pricing" (goes to the new pricing section on the homepage) | The label promises prices. |
| "Changelog" + 5 social icons (all go to "#") | Remove until they exist | Dead links read as an abandoned product. |
| "Contact Us", "Help Center", "Terms of Service" | "Contact us", "Help center", "Terms of service" | Sentence case everywhere. |
| "© 2026 MyFit Inc. Made for fit-obsessed merchants." | [VERIFY] "© 2026 MyFit Inc." against App Store developer "Redcircle Digital". If both are correct: "MyFit is made by Redcircle Digital." | Merchants who cross-check will notice the two names. |

---

## 11. Metadata

- Page title
  - Current: "Shopify Size Quiz App for Apparel Merchants"
  - Proposed: "MyFit: Size quiz app for Shopify apparel stores"
  - Why: the brand name is missing from tabs, bookmarks and search results.
- The meta description has the same "visual" and "exact" problems. Align it with the new subhead.

---

## Facts to confirm before shipping (blocking)

1. ~~Language count~~ **Confirmed 2026-11-04: 40+ languages, including right-to-left.** Update the Shopify App Store listing, which still shows 5.
2. Does the quiz have visual steps?
3. Theme support: only Online Store 2.0 themes, or vintage themes too?
4. Is brand matching automatic or set by the merchant? Does the Free plan show a "Powered by MyFit" mark?
5. Are the logos current customers?
6. Sources for 42% / $25+ / 52%.
7. How "returns prevented" is measured.
8. Does Unlimited include advanced analytics? What counts as one "quiz"? (Prices themselves confirmed 2026-11-04: Free 25 quizzes/month, Unlimited $4/month, 14-day trial.)
9. Script weight, for the speed FAQ.
10. Shopper data storage, retention and GDPR status.
11. MyFit Inc. vs Redcircle Digital.
12. Is phone number needed on the demo form?
