# Ariapura — Growth Plan 90 giorni

**Obiettivo:** trasformare Ariapura da sito statico passivo a **funnel a circuito chiuso** che genera 80-150 lead qualificati/mese a regime.
**Stack:** GHL + n8n self-host + CallRail + Cal.com + Vercel LP + WP core.
**Investimento mensile a regime:** ~€152/mese tooling + adv budget cliente (€800-2.500/mese consigliato).

---

## 1. Funnel a circuito chiuso · diagramma

```
┌─────────────────────────────────────────────────────────────────────────┐
│  ACQUISITION                                                            │
│  ┌───────────┐  ┌───────────┐  ┌───────────┐  ┌──────────┐              │
│  │ Google    │  │ SEO local │  │ GMB       │  │ Referral │              │
│  │ Ads       │  │ + AEO     │  │ Castel    │  │ B2B      │              │
│  │ Search    │  │ ariapura  │  │ Maggiore  │  │          │              │
│  └─────┬─────┘  └─────┬─────┘  └─────┬─────┘  └────┬─────┘              │
│        │              │              │              │                    │
│        └──────────────┴──────────────┴──────────────┘                    │
│                            ↓                                            │
└────────────────────────────┼────────────────────────────────────────────┘
                             ↓
┌─────────────────────────────────────────────────────────────────────────┐
│  CONVERSION (Vercel LP settoriale + form / WhatsApp / call)             │
│                                                                         │
│  /clinica · /uffici · /horeca · /scuola · /industria · /residenziale    │
│  + ariapura.org/listino · /sopralluogo                                  │
└────────────────────────────┼────────────────────────────────────────────┘
                             ↓
┌─────────────────────────────────────────────────────────────────────────┐
│  CRM (GHL)                                                              │
│                                                                         │
│  Pipeline: Nuovo Lead → Sopralluogo Pianificato → Sopralluogo Fatto     │
│         → Preventivo Inviato → Trattativa → Vinto / Perso               │
│                                                                         │
│  Tag: settore · provincia · canale · valore stimato                     │
└────────────────────────────┼────────────────────────────────────────────┘
                             ↓
┌─────────────────────────────────────────────────────────────────────────┐
│  AUTOMATION (n8n self-host)                                             │
│                                                                         │
│  • Triage lead (smart routing per settore + provincia)                  │
│  • Auto-conferma sopralluogo (SMS + email + WA)                         │
│  • Auto-PDF report sopralluogo entro 48h                                │
│  • Reminder sequence (24h pre-sopralluogo, 24h post-preventivo)         │
│  • Recensione GMB request post-vittoria (loop SEO)                      │
└────────────────────────────┼────────────────────────────────────────────┘
                             ↓
┌─────────────────────────────────────────────────────────────────────────┐
│  RETENTION + LOOP                                                       │
│                                                                         │
│  • Recensione GMB → SEO local boost → più lead                          │
│  • Caso anonimizzato → social drip → trust                              │
│  • Piano di mantenimento → MRR contratti annuali                        │
│  • Referral B2B → upsell case multi-sede                                │
└─────────────────────────────────────────────────────────────────────────┘
```

---

## 2. Roadmap 90 giorni

### Fase 1 — Settimana 1-2 · Fondamenta (Phase 1 contract)

**Obiettivo:** stop the bleeding. Riparare audit gaps critici.

- [ ] SSL fix bare-domain (Cloudflare full-strict)
- [ ] Redirect 301 `/servizi/` → `/servizi/sanificazione`
- [ ] NAP confermato + applicato GMB + sito + Reteimprese + LinkedIn
- [ ] P.IVA + REA + albo iscrizione in footer + privacy
- [ ] Schema JSON-LD (LocalBusiness + HVACBusiness + FAQPage) su tutte le pagine principali
- [ ] LP variant scelta (V1-V5) deployed su `ariapura.org` o subdomain
- [ ] Web3Forms → SMTP cliente per delivery affidabile
- [ ] Form embed su LP + form principale ariapura.org
- [ ] GMB Castel Maggiore riottimizzato (foto + post + categoria primaria + secondaria)
- [ ] Plausible/GA4 + GTM installati

**KPI fine fase 1:** 0 errori 4xx/5xx · 100% schema valid · GMB profile complete >95% · lead form ricevente.

### Fase 2 — Settimana 3-6 · Acquisition (LP settoriali + GMB + Ads)

**Obiettivo:** turn on traffic.

- [ ] 6 LP settoriali deployed (Vercel, riprende design variant scelto)
- [ ] Google Ads campaign Search · 3 ad groups (cliniche / uffici / HoReCa) · €800/mese budget di partenza
- [ ] CallRail tracking numbers attivati per LP + GMB
- [ ] Cal.com booking sopralluogo embed in tutte le LP
- [ ] WhatsApp Business API + click-to-chat su ogni LP
- [ ] GHL pipeline configurata (6 stage + tagging settore/provincia)
- [ ] n8n flow #1: triage lead da form → assegnazione settore → notifica
- [ ] n8n flow #2: SMS/email auto-conferma + reminder
- [ ] Editorial calendar GBP post (3/sett · prima/dopo cantieri anonimizzati)

**KPI fine fase 2:** 25-40 lead/mese · CPL <€35 · GMB views +50%.

### Fase 3 — Settimana 7-10 · Automation depth (PDF report + nurture)

**Obiettivo:** convert smarter, not harder.

- [ ] n8n flow #3: auto-PDF report post-sopralluogo (template Letterpress) entro 48h
- [ ] n8n flow #4: nurture sequence settoriale (5 email/14 giorni per ogni settore)
- [ ] WhatsApp template approvati Meta (sopralluogo confermato, preventivo pronto, post-intervento)
- [ ] Recensione GMB request automatizzata 7gg post-vittoria
- [ ] Case study anonimizzati pubblicati (3 minimo) — alimentano social + LP
- [ ] Blog revival: 2 articoli/mese (pillar SEO + AEO long-tail)
- [ ] Editorial drip social (LI + IG + FB) settimanale
- [ ] Heatmap Hotjar/Microsoft Clarity sulle LP per ottimizzare CTA

**KPI fine fase 3:** 50-90 lead/mese · close rate >25% · 2-3 recensioni GMB nuove/mese.

### Fase 4 — Settimana 11-13 · Scale + retention loop

**Obiettivo:** lock in MRR + scale ads.

- [ ] Piano di mantenimento annuale (contratto 12 mesi, fatturato split semestrale)
- [ ] Programma referral B2B (commercialisti, property manager, ristoratori partner)
- [ ] Lookalike Audience FB Ads + Google Display retargeting
- [ ] Espansione GMB satellite Modena + Ferrara (2 nuovi listing se pertinente)
- [ ] CallRail call analytics → ottimizzazione orari + script telefonico
- [ ] Recensione → caso anonimizzato → social drip (loop chiuso)

**KPI fine fase 4:** 80-150 lead/mese · MRR contratti annuali su 30%+ clienti vinti · Cost per Acquisition stabile · 8+ recensioni GMB/mese.

---

## 3. Stack tooling · costi mensili

| Tool | Funzione | Costo mensile |
|------|----------|---------------|
| GHL Agency Plan | CRM + pipeline + WhatsApp + email + booking | €97-297 |
| n8n self-host (VPS Hetzner CX22) | Automation server | €10 |
| CallRail Italia (basic) | Call tracking | €45 |
| Cal.com self-host | Booking sopralluogo | €0 (su VPS già pagato) |
| Plausible Cloud | Analytics privacy-first | €9 |
| Hotjar / Clarity | Heatmap | €0-39 (Clarity gratis) |
| Web3Forms / SMTP cliente | Form delivery | €5-15 |
| Vercel Pro | LP hosting | €20 |
| Cloudflare Free | CDN + SSL | €0 |
| **Totale tooling** | | **~€150-330/mese** |
| **Adv budget consigliato** | Google Ads + Meta | **€800-2.500/mese** |

---

## 4. KPI projection · lead/mese

| Periodo | Lead/mese (range) | Note |
|---------|-------------------|------|
| Pre-intervento (oggi) | 8-15 | stima da audit + traffico organico esistente |
| Fine fase 2 (settimana 6) | 25-40 | LP + Ads + GMB ottimizzato |
| Fine fase 3 (settimana 10) | 50-90 | nurture + PDF auto + case studies |
| Fine fase 4 (settimana 13) | 80-150 | retention loop + scale ads |
| **Stato a regime mese 6+** | **120-200** | dipende da budget adv cliente |

**Assumptions:**
- CPL Google Search HVAC Bologna: €25-40
- Close rate post-sopralluogo: 30-45%
- Average ticket cliniche/hotel: €4.500-7.500
- Average ticket residenziale: €450-700
- LTV cliente con piano mantenimento: €8.000-22.000

---

## 5. Pricing SkynetLabs (interno · non per cliente)

### Phase 1 — Fondamenta (settimana 1-2)
- Una tantum: **€2.400-3.200**
- Include: SSL/404/NAP/P.IVA fix · LP scelta deployed · schema · GMB ottimizzato · GA4/Plausible setup

### Phase 2 — Acquisition (settimana 3-6)
- Una tantum: **€3.800-5.200**
- Include: 6 LP settoriali · Ads setup + 30gg gestione · CallRail · GHL pipeline · n8n triage flow

### Phase 3 — Automation (settimana 7-10)
- Una tantum: **€2.400-3.400** + retainer **€600-1.000/mese** (gestione)
- Include: n8n flows depth · PDF auto · nurture sequences · WhatsApp templates · case studies · blog revival

### Phase 4 — Scale (mese 4+)
- Retainer mensile: **€1.200-2.400/mese**
- Include: ads management · n8n maintenance · contenuti social · recensioni loop · reportistica

### Pacchetto completo 90 giorni
- Range: **€11.000-16.000 setup** + retainer mese 4+ (€1.200-2.400/mese)
- ROI atteso break-even: mese 5-7

---

## 6. Risk + mitigation

| Rischio | Mitigazione |
|---------|-------------|
| Cliente non ha P.IVA pronta in 7gg | Phase 1 può procedere su altri item, blocco tecnico isolato |
| Foto reali cantieri non disponibili | Variant scelto rimane su Unsplash hotlink fino a fornitura cliente |
| Budget Ads troppo basso | Riprioritizzare SEO + GMB · Ads in fase 3 |
| Cognome Alex non disponibile | "Alex, fondatore" mantenuto fino a contratto |
| Conflict NAP non risolto | Default Castel Maggiore + cita Bologna come "ufficio commerciale" |
| Stack già esistente incompatibile (no GHL) | Adattare a Hubspot/Brevo/Pipedrive · pricing si alza 15% |

---

## 7. Hand-off finale (mese 13+)

- Cliente possiede: GHL account · n8n VPS · LP code Vercel · GMB · ads accounts · documentazione
- SkynetLabs offre: retainer manutenzione (€600-1.200/mese) o hand-off completo con SOP scritti
- Tempo medio hand-off: 30 giorni con shadowing operatore interno cliente

---

Documento interno SkynetLabs. Versione condivisa con cliente solo dopo firma Phase 1.
