# Changelog

All notable changes to this project are documented in this file.
The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.1.0/).

## [2026.10] - 2026-10-12

- skynetlabs-ariapura-cinema is a public speculative pitch demo for Ariapura (HVAC air-duct sanitisation, Bologna): one index.html with five cinematic variants plus Italian pitch documents in docs/.
- State: no commits since the 2026.09 release (2026-09-16); last functional commit 2026-05-08 added the short Italian outreach variant. Markup and deploy config were not touched.
- Reviewed October 2026: README, commit history and link check; the stated live URL https://skynetlabs-ariapura-cinema.vercel.app returns 200; a Work with SkynetLabs section was added.
- Known gaps, stated in the repo: robots.txt is Disallow: / because the pitch is speculative; Web3Forms key is a placeholder; founder surname and P.IVA unfilled; client photos not swapped in; no LICENSE; still waiting on the client to pick a variant.

## [2026.09] - 2026-09-16

- Maintenance review of skynetlabs-ariapura-cinema — a speculative pitch demo by SkynetLabs for Ariapura (HVAC air-duct sanitisation, Bologna, Italy); the README states it deprecates `skynetlabs-ariapura-relaunch`.
- Status: one static `index.html` holding five visually distinct cinematic variants (V1 Aether / V2 Solomeo / V3 Cleanroom / V4 Terra Nuova / V5 Cinecitta) with a top-right switcher persisted in `localStorage`. Stack is CDN-only: Tailwind, Google Fonts, Three.js 0.160 (lazy-initialised for V1), Web3Forms, plus LocalBusiness/HVACBusiness/FAQPage JSON-LD. README states the live URL as https://skynetlabs-ariapura-cinema.vercel.app.
- Pitch material is versioned in `docs/`: RESEARCH.md (audit gaps and competitor map), GROWTH-PLAN.md (90-day funnel), CLIENT-MESSAGE.md and CLIENT-MESSAGE-SHORT.md (Italian, Lei register), CLIENT-PITCH.md. Last commit was 2026-05-08, adding the short Italian outreach variant.
- Reviewed September 2026: docs refreshed, versioned as v2026.09. No markup, variant or deploy-config changes in this release.
- Known gaps, all pre-existing and stated in the repo: `robots.txt` is `Disallow: /` because the pitch is speculative; the Web3Forms key is still a placeholder; founder surname and P.IVA are unfilled; client photos are not yet swapped in; no LICENSE; no CHANGELOG.md before this release. The repo is still waiting on the client picking one of the five variants.
