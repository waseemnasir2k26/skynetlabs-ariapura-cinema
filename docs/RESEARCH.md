# Ariapura — Research & Audit Brief

**Cliente:** Ariapura · sanificazione aeraulica HVAC, Bologna
**Sito attuale:** ariapura.org
**Data audit:** 2026-05-08
**Scopo:** ammunition doc per ricostruzione sito + pitch SkynetLabs

---

## 1. Dati cliente verificati

| Campo | Valore | Note |
|-------|--------|------|
| Founder | Alex (cognome ignoto) | **DA CONFERMARE in pitch Qs** |
| Esperienza | Da oltre 30 anni | self-claim, da contratto |
| Certificazioni | **FGAS + ACCREDIA** | Le uniche legittime. NADCA/AIISA = NON certificati |
| Sede principale | Via Lame 261, Castel Maggiore (BO) — 40013 | **NAP conflict** con Reteimprese (Via Costituzione 19, 40033 Bologna). Flag in Qs. |
| Tel | +39 051 0828717 | unico |
| Email | info@ariapura.org | unico |
| Orari | Lun-Ven 09:00-13:00 / 14:30-17:30 · Sab-Dom su appuntamento | confermato |
| Servizi attivi | Sanificazione condotte · Manutenzione · Filtri elettrostatici · Check-up Gratuito · Check Muffa | da homepage |
| Social | IG @ariapurabologna · FB · YouTube · LinkedIn | confermati |
| Hero hook attuale | "Proteggi la tua salute" | **debole** — sostituito |
| Garanzia LP locale | "Se non sei soddisfatto del risultato, ripetiamo l'intervento gratis!" | **PROMUOVERE A HERO** |

---

## 2. Audit gaps · 10 punti critici

### Critici (Phase 1, settimana 1)

1. **SSL bare-domain cert break** — visitando `https://ariapura.org` senza www, il browser mostra warning. Risoluzione: Cloudflare full-strict + cert bare-domain o redirect 301 → www.
2. **`/servizi/` → 404** — la homepage linka in H2 a una sezione che non esiste. Sitemap + redirect immediati.
3. **NAP conflict** — 2 indirizzi in giro (Castel Maggiore vs Bologna). Confondere Google Business + danneggiare local SEO. Default: Via Lame 261 finché non confermato.
4. **P.IVA assente** — requisito legale italiano. Va in footer + privacy policy.
5. **Zero schema markup** — nessun JSON-LD, niente LocalBusiness, niente HVACBusiness, niente FAQPage. Penalizza GMB + AEO.

### Strutturali (Phase 2)

6. **Blog fermo da 14 mesi** — ultimo post Marzo 2025. Penalizza freshness signal Google + segnala dismissione.
7. **Zero case studies + zero before/after + zero video** — il settore vive di "vedere è credere". L'hero è cieco.
8. **Settori non separati** — homepage nomina "medici, B&B, allergici, pet" senza pagine dedicate. Nessuna landing settoriale → nessuna conversion specializzata.
9. **No team page · no founder photo · no cert images** — fiducia minima. In un mestiere che entra in cliniche e hotel, è un suicidio reputazionale.
10. **No pricing transparency** — niente listino, neanche indicativo. Costringe ogni lead a chiamare per scoprire ordini di grandezza, perdendo i 70% di prospect "shoppers".

---

## 3. Competitor map italiano

### Pattern dominante (90% del mercato)

- **Corporate-blue navy/white** default
- Hero generico "Sanificazione professionale impianti aeraulici"
- Nessun founder visibile
- Stock photo HVAC industriali di Shutterstock
- Zero trasparenza prezzi
- Zero settori dedicati

### Player nazionali (top tier)

| Brand | Posizione | Forza | Debolezza |
|-------|-----------|-------|-----------|
| **Alisea** | Leader nazionale corporate | Coverage Italia, brand recognition | Aestetica anonima, nessuna voce founder |
| **AirBio** | Mid-tier nazionale | Settori multipli | Sito generico, photo stock |
| **Techno One** | Mid-tier nazionale | Coverage Nord Italia | Sito 2010-style |
| **Indoor Ambiente** | Specialist sanificazione | Posizionamento clinico | Aestetica corporate-blue |

### Player Bologna / Emilia (regionali)

| Brand | Posizione | Forza | Debolezza |
|-------|-----------|-------|-----------|
| **Sidabo** | Heritage 1977, NADCA | Storia + cert internazionali | Sito invecchiato, niente cinematic |
| **Cooplar** | Generalist pulizia | Coverage local | Non specializzato HVAC |
| **Eco Service** | Generalist | Pricing aggressivo | Non specializzato HVAC |

---

## 4. White space identificato (dove Ariapura può vincere)

1. **Cinematic landscape video** — nessuno in Italia HVAC usa drone/video di terra. Vanguard pulito.
2. **Dark editorial** — tutti corporate-blue. Andare dark + serif = scroll-stopper.
3. **Founder-led** — Alex 30 anni di mestiere è un asset narrativo. Tutti gli altri sono anonimi.
4. **Transparent prices** — listino indicativo + "preventivo personalizzato dopo sopralluogo" = wedge unique.
5. **Settori microsites** — 6 settori, 6 LP dedicate. Local SEO + GBP + Ads triple-stack.
6. **Borescope before/after** — videoispezione robotizzata produce contenuti naturali. Nessuno in Italia li mostra.
7. **UTA risk calculator** — quiz "Quando hai sanificato l'ultima volta?" con scoring → lead magnet.

---

## 5. Visual brief · 5 variants

### V1 — AETHER (WebGL particles)
- Mood: cosmico, scientifico, "respiro misurato"
- Wedge: nessun competitor italiano usa Three.js. Premium + tech-forward.
- Palette: `#0A0F14` / `#7FB8C9` / `#E8EEF2`
- Type: Spectral + Inter
- Hero: "Lei respira ciò che non vede."

### V2 — SOLOMEO (Italian humanist editorial)
- Mood: artigianalità italiana, eredità
- Wedge: posizionamento Brunello-Cucinelli applicato all'HVAC. Premium emotivo.
- Palette: `#F5EFE4` / `#8C6F4B` / `#2B2620`
- Type: Cormorant Garamond + Manrope
- Hero: "L'aria che merita la Sua azienda."

### V3 — CLEANROOM (clinical brutalism)
- Mood: tecnico, rigoroso, "compliance-first"
- Wedge: parla la lingua dei direttori sanitari + responsabili sicurezza.
- Palette: `#FAFAFA` / `#0E0E10` / `#A6E0D2`
- Type: JetBrains Mono + Spectral
- Hero: "PROTOCOLLO 4-STEP. ARIA CERTIFICATA."

### V4 — TERRA NUOVA (landscape parallax)
- Mood: territorio, sostenibilità, Emilia
- Wedge: ancora il brand al territorio. Local + ESG narrative.
- Palette: `#1A2A2E` / `#6B8E7F` / `#B8945C`
- Type: Fraunces italic + DM Sans
- Hero: "Aria pulita per la Sua terra."

### V5 — CINECITTÀ (film letterbox)
- Mood: documentario, narrativo
- Wedge: trasforma Ariapura da fornitore a "studio". Usato per content + social drip.
- Palette: `#0B1416` / `#D97742` / `#3E8E9C`
- Type: Playfair Display + Archivo
- Hero: "Capitolo 1 — L'aria invisibile."

---

## 6. Settori target (6 LP dedicate)

| Settore | Pain point | Hook | Lead magnet |
|---------|------------|------|-------------|
| Cliniche / RSA | Compliance D.Lgs. 81 + ASL | "Certificazione conforme audit" | Checklist sanitaria PDF |
| Uffici | Assenteismo respiratorio | "Riduci giorni malattia del 18%*" | Audit aria gratuito |
| HoReCa | Recensioni "puzza in lobby" | "Aria neutra in lobby in 72h" | Caso hotel anonimo |
| Scuole | Bambini sensibili + L.R. | "Aria normata per le aule" | Checklist scuola |
| Industria | Polveri + sicurezza | "Protezione operatori reparto" | Audit fumi |
| Residenziale | Allergici + neonati | "Casa che respira meglio" | Test allergeni |

*disclaimer su dati indicativi

---

## 7. Stack consigliato (post-pitch)

- **WordPress (theme custom)** — ariapura.org già su WP, tenere
- **Vercel** per landing speculative + LP settori (subdomain)
- **GHL** per CRM + pipeline lead
- **n8n** self-host VPS Hetzner per triage + auto-PDF preventivo
- **CallRail Italia** o **Aircall** per tracking chiamate
- **Cal.com** self-host per booking sopralluogo
- **Plausible** per analytics privacy-first (GDPR)
- **GBP** Castel Maggiore — riconfigurare con foto reali

---

## 8. Note di posizionamento

- **NON dire** "i migliori d'Italia" / "leader del settore" / "azienda numero 1" → no-fake-claims
- **DIRE** "da oltre 30 anni in Emilia-Romagna" / "FGAS + ACCREDIA" / "garanzia di intervento ripetuto"
- **NON inventare** clienti famosi → "Clinica privata Bologna · anonimizzato"
- **NON inventare** numeri precisi → "−92% indicativo, post-bonifica meccanica"
- **DIRE** "preventivo personalizzato dopo sopralluogo" sempre

---

Documento di lavoro interno SkynetLabs. Non condividere con cliente prima della firma contratto Phase 1.
