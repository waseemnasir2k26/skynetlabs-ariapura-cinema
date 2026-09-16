# Ariapura — 5 Piste Cinematografiche (Speculative Pitch)

> **DEPRECATES** `skynetlabs-ariapura-relaunch`. This is the cinema-grade replacement bundle.

## Status

Last reviewed: September 2026 · release v2026.09

Speculative pitch demo for **Ariapura** — sanificazione aeraulica HVAC, Bologna. 5 visually distinct cinematic variants in a single HTML file with a top-right switcher.

- **Live URL (after deploy):** `https://skynetlabs-ariapura-cinema.vercel.app`
- **Client site:** ariapura.org
- **Sede:** Via Lame 261, Castel Maggiore (BO)
- **Tel:** +39 051 0828717
- **Founder:** Alex (cognome da confermare)

## The 5 Variants

| # | Name | Aesthetic | Hero | Stack |
|---|------|-----------|------|-------|
| V1 | **Aether** | WebGL particle field, dark void | "Lei respira ciò che non vede." | Three.js r160 CDN |
| V2 | **Solomeo** | Italian humanist editorial, cream + brass | "L'aria che merita la Sua azienda." | Cormorant + Manrope, Ken-Burns CSS |
| V3 | **Cleanroom** | Clinical brutalism, mono | "PROTOCOLLO 4-STEP. ARIA CERTIFICATA." | JetBrains Mono + Spectral |
| V4 | **Terra Nuova** | Landscape parallax, sage + brass | "Aria pulita per la Sua terra." | Fraunces italic + DM Sans |
| V5 | **Cinecittà** | 2.39:1 letterbox, teal-orange grade | "Capitolo 1 — L'aria invisibile." | Playfair + Archivo |

## What's inside

- `index.html` — single-file build, all 5 variants, top-right switcher (V1-V5), state persisted via `localStorage`
- `docs/RESEARCH.md` — audit gaps + competitor map + visual brief
- `docs/GROWTH-PLAN.md` — 90gg closed-loop funnel (Ads/SEO/GMB → LP → form → GHL CRM + n8n triage → preventivo → recensione GMB)
- `docs/CLIENT-MESSAGE.md` — paste-ready Italian pitch (Lei register)
- `docs/CLIENT-PITCH.md` — pitch log + scope Qs + pre-send checklist
- `vercel.json` — clean URLs config
- `robots.txt` — `Disallow: /` (speculative — flip on client confirm)

## Stack

- Tailwind CDN
- Google Fonts (Spectral, Inter, Cormorant Garamond, Manrope, JetBrains Mono, Fraunces, DM Sans, Playfair Display, Archivo)
- Three.js 0.160 CDN (V1 Aether particle field — only initialized when V1 is active)
- Web3Forms for contact submissions (placeholder key — swap before live)
- Schema.org JSON-LD: `LocalBusiness` + `HVACBusiness` + `FAQPage`

## Pre-deploy checklist

1. Replace `REPLACE_WITH_WEB3FORMS_KEY` (5 occurrences — one per variant form) with real Web3Forms access key
2. Confirm sede with client (Via Lame 261 vs Reteimprese listing Via Costituzione 19)
3. Add P.IVA in footer (currently "P.IVA da confermare")
4. Swap Unsplash hotlink images for client-provided real photos (cantieri, attrezzature, founder ritratto)
5. Pick 1 variant as production candidate after client review
6. Flip `<meta name="robots" content="noindex, nofollow">` and `robots.txt` once selected variant is approved
7. Add P.IVA + REA + iscrizione albo (Italian legal req)

## Deploy

```bash
cd C:\Users\info\OneDrive\Desktop\GITHUB\skynetlabs-ariapura-cinema
git init
git add -A
git commit -m "Initial cinema bundle: 5 cinematic variants for Ariapura speculative pitch"
gh repo create waseemnasir2k26/skynetlabs-ariapura-cinema --public --source=. --remote=origin --push
vercel --prod
```

## Hard constraints honoured

- 100% Italian Lei register
- Only certifications cited: **FGAS + ACCREDIA** (no fake NADCA/AIISA)
- All case studies anonimizzati (no invented client names/logos)
- All pricing as **indicative ranges** with disclaimer
- No fabricated metrics (the −92% / −97% / +18% in V3 carry explicit "indicativo" disclaimer)
- Free guarantee preserved: "Se non sei soddisfatto, ripetiamo l'intervento gratis"
- 30+ anni framed as "Da oltre 30 anni" (self-claim, conservative)

## Audit gaps baked as wedges

1. SSL bare-domain cert break — fix in Phase 1 (Cloudflare/cert)
2. /servizi/ 404 — sitemap + redirects in Phase 1
3. NAP conflict (2 addresses) — flagged in pitch Qs
4. P.IVA missing — legal requirement, footer fix Phase 1
5. Blog dead 14 months — Phase 2 editorial revival
6. Zero schema markup — baked into all 5 variants
7. Zero case studies / before-after — V3/V4 templates ready for client photos
8. No settori split — 6 settori cards in every variant
9. No team page — V2/V4 founder-letter templates ready
10. No pricing transparency — listino indicativo in every variant

## Niche white-space exploited

- 90% Italian competitors are corporate-blue → all 5 variants AVOID navy/white
- Italian leaders (Alisea, AirBio, Techno One, Indoor Ambiente) all corporate-top → we go founder-led + cinematic
- Bologna regional thin (Sidabo NADCA / Cooplar / Eco Service) → we own dark-editorial + transparent prices

## Next session

- Client picks 1 variant from V1-V5
- Swap real photos
- Fill founder cognome + P.IVA
- Flip noindex
- Push to ariapura.org via Phase 1 contract
