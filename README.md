# MyFit landing page (redesign proposal)

A standalone static rebuild of the myfitsize.com landing page. It applies the
findings of the November 2026 UX critique and audit. It is a design proposal,
not the production site: the live site's source code is maintained elsewhere.

## View it

Open `index.html` in a browser. No build step or server is needed.

To serve it locally (optional):

```bash
python3 -m http.server 8000
```

Then open http://localhost:8000.

## What's in here

| Path | What it is |
|---|---|
| `index.html` | The full page: markup, styles and the small amount of JavaScript (setup-step tabs, demo video, mobile menu, sticky mobile install bar, form validation). |
| `assets/img/` | Images copied from myfitsize.com and converted to resized WebP (2.6 MB down to about 0.4 MB). |
| `assets/media/demo.mp4` | The shopper demo recording. |
| `docs/critique-2026-11-04.md` | Summary of the critique and audit scores and priority issues. |
| `docs/copy-deck.md` | Every copy change, with the reason for it, plus the facts still to confirm. |
| `.impeccable/config.json` | Design-scan settings, including two reviewed false positives. |

## Before this can ship

Yellow tags on the page mark facts that only the MyFit team can confirm, such
as the language count, theme support, stat sources, shopper data handling, and
company name. The full list is at the end of `docs/copy-deck.md`.

Links to Help center, Contact, Privacy and Terms point at the live
myfitsize.com pages. Install buttons go to the real Shopify App Store listing.
The walkthrough form validates input but does not send anything yet. To connect
it, set `data-endpoint` on `<form id="walkthrough-form">` to a URL that accepts a
JSON `POST` with `firstName`, `email`, `store` and `plan`. The form already
handles the sending state, double submits, timeouts (`data-timeout`, default
15 seconds), 4xx, 429 and 5xx responses, and offline errors, and keeps what the
visitor typed. A hidden honeypot field (`company_website`) quietly drops bot
submissions. Validate again on the server; the browser checks are only a
convenience.
