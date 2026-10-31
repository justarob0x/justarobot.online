# NEXT — justarobot.online (developer site, GitHub Pages)

## 2026-10-31 — Spanish page /es/ (STATUS: live on push)

`es/index.html` (lang es, formal usted): EU Compliance Kit card first and in full (links eucompliance /es and /es/reglas, facts
copied from the EN card); DATEV/BMD/LUCID/Buchungsstapel/plugin/E-Rechnung/CutSheetPro as short neutral cards. hreflang es +
og:locale es_ES + "Español" switcher on EN and DE; Kit language row adds Spanish on all three; sitemap 2026-10-31 with /es/.

## 2026-10-19 — LUCID Verpackungsgesetz Report card (STATUS: live, 46fb820 + og 988268d)

EPR app (approved + published 19 Oct) card EN + DE after BMD-Export: packaging quantities for LUCID (VerpackG) and ARA
from shipped Shopify orders, CSV/PDF, $11.99/month + 14-day trial; listing
https://apps.shopify.com/lucid-verpackungsgesetz-report (DE card links the same URL, like BMD) and demo
https://youtu.be/FDCi8ZxmkYo; site epr.justarobot.online; icon `lucid.png` (192, from epr-report
`docs/listing/icon-1200.png`). Meta/OG/Twitter descriptions name it; aside "three are Shopify apps"; sitemap 2026-10-19.
og.png re-rendered: 7 icons at 126px (DATEV, BMD, LUCID, EU Kit, Buchungsstapel, E-Rechnung, CutSheetPro), names line
wraps to two lines; source HTML in the epr-report session scratchpad `og/og.html`. Closes pass-2 item 3 below.

## 2026-10-15 — BMD-Export card (STATUS: live, 2dc87d2)

BMD-Export (Austrian Shopify app, approved 15 Oct) card EN + DE after Export für DATEV: BMD NTCS / RZL, EKR, listing
https://apps.shopify.com/bmd-export-2 and walkthrough https://youtu.be/FppHEJGvU10; icon `bmd.png` (192, from
datev-export `docs/listing/icon-bmd.png`). Meta/OG/Twitter descriptions name it; aside "two are Shopify apps".
og.png re-rendered 15 Oct: 6 icons (DATEV, BMD, EU Kit, Buchungsstapel, E-Rechnung, CutSheetPro) + names line
("Export für DATEV", old "DATEV-Export" fixed); source HTML in the datev-export session scratchpad `og/og.html`.

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
1. DONE 20 Oct (d60079a): EU Kit card now ten rules (nine on Wix), Shopify install link + pricing + price fix /
   email alert / PDF record; green claims + passports stay Wix-only (the Shopify app has neither). Was: Shopify verdict (~15–16 Oct): EU Kit card "on Wix" → "on Wix and Shopify" for green claims + passports; add
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
