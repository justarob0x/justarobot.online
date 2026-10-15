# NEXT — justarobot.online (developer site, GitHub Pages)

## 2026-10-15 — BMD-Export card (STATUS: live, 2dc87d2)

BMD-Export (Austrian Shopify app, approved 15 Oct) card EN + DE after Export für DATEV: BMD NTCS / RZL, EKR, listing
https://apps.shopify.com/bmd-export-2 and walkthrough https://youtu.be/FppHEJGvU10; icon `bmd.png` (192, from
datev-export `docs/listing/icon-bmd.png`). Meta/OG/Twitter descriptions name it; aside "two are Shopify apps".
OPEN: og.png still has 5 icons (no BMD) — re-render.

## 2026-10-13 — App cards updated for E-Rechnung, green claims, product passports (STATUS: live; pass 2 waits on store verdicts)

**DONE / LIVE** (d7e78cb, 8be465d, pushed = deployed by GitHub Pages in ~1–2 min)
- New **E-Rechnung** card (EN + DE): Sheets & Excel add-on, XRechnung/ZUGFeRD, 30-day trial, link to the free
  viewer https://erechnung.justarobot.online/xrechnung-oeffnen. Icon `erechnung.png` = erechnung-sheets
  `docs/listing/icon-128.png`. No install buttons yet.
- **EU Compliance Kit** card: green-claims check line (EU rules since 27 Sep 2026, free on Wix) and digital product
  passports line (Pro on Wix, EU battery passport from Feb 2027).
- Meta/OG/Twitter descriptions (EN + DE) name all apps; intro "aside" mentions the Sheets/Excel add-on.
- `og.png` re-rendered: 5 icons (DATEV, EU Kit new € icon, Buchungsstapel, E-Rechnung, CutSheetPro) + full names line
  (old one cut its text off and had the old EU icon). Sitemap lastmod 2026-10-13.

**OPEN — pass 2 (waiting on others)**
1. Shopify verdict (~15–16 Oct): EU Kit card "on Wix" → "on Wix and Shopify" for green claims + passports; add
   Shopify install link. Green-claims section on eucompliance.justarobot.online goes out with the Shopify
   merge/deploy (same Railway service as the app under review).
2. Google Marketplace approved 13 Oct: "Add to Google Sheets" link + body link on the E-Rechnung card (EN + DE) live
   14 Oct. Still open: Microsoft AppSource link once certified; Google link on erechnung.justarobot.online + Wissen.
4. Buchungsstapel G2 profile (listed 12 Oct): g2.com blocks curl (403), URL unverified — add a link once Bill
   confirms the profile URL.
3. EPR report (App Store review): add a card + icon once approved.

**Gotchas**
- og.png render: HTML in scratchpad + Playwright `chromium.launch(channel="chrome")` (bundled headless shell not
  installed); 1200×630.
- German copy uses non-breaking hyphens (U+2011) in compounds (`Add‑on`, `E‑Rechnung`); keep them.
- Verify deploy by fetching the live page with a cache-busting query and grepping the new text.
