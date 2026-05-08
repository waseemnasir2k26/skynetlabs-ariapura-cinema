# Ariapura · Pitch log + Scope Qs + Pre-send checklist

**Cliente:** Ariapura · sanificazione aeraulica HVAC, Bologna
**Approccio:** speculative-build → pitch (validato 2026-04-22 pattern, vedi `feedback-speculative-build-pitch.md`)
**Status:** demo built · pitch ready · awaiting send

---

## 1. Pitch log

| Data | Evento | Owner | Status |
|------|--------|-------|--------|
| 2026-05-08 | 5 cinematic variants built (this repo) | SkynetLabs/Waseem | ✅ |
| 2026-05-08 | RESEARCH.md + GROWTH-PLAN.md compiled | SkynetLabs | ✅ |
| 2026-05-08 | CLIENT-MESSAGE.md drafted (Lei register) | SkynetLabs | ✅ |
| 2026-05-08 | Pre-send checklist outstanding | Waseem | ⏳ |
| TBD | Push to github.com/waseemnasir2k26/skynetlabs-ariapura-cinema | Waseem | ⏳ |
| TBD | Vercel deploy production | Waseem | ⏳ |
| TBD | Smoke test 5 variants in incognito | Waseem | ⏳ |
| TBD | Send pitch email to info@ariapura.org | Waseem | ⏳ |
| TBD+72h | Follow-up if no reply (competitor SEMrush angle) | Waseem | ⏳ |

---

## 2. Scope-unlocking questions (verbatim, copy from CLIENT-MESSAGE.md)

> 7 questions in pitch + 1 pricing-lever question = 8 total

### 1. Pista preferita
**Quale variant La convince di più al primo sguardo?**
- V1 Aether (WebGL, dark, scientifico)
- V2 Solomeo (italian humanist, founder-letter)
- V3 Cleanroom (clinical brutalism, mono)
- V4 Terra Nuova (landscape, sage+brass)
- V5 Cinecittà (letterbox, narrative chapters)
- Misto valido (es: hero V2 + processo V3)

→ **Decision impact:** locks down design system per 6 LP settoriali in fase 2

### 2. Cognome fondatore
**Il Suo cognome.**
- Nei copy ho lasciato "Alex, fondatore"
- Vorrei firmare la lettera del fondatore con nome e cognome reali

→ **Decision impact:** founder authority + LinkedIn Sales Navigator outreach futuro

### 3. P.IVA + REA + albo
**Avete già P.IVA + numero REA + iscrizione albo (se applicabile)?**
- Requisito legale italiano
- Schema markup completo li include

→ **Decision impact:** compliance + trust + Google Business Profile

### 4. NAP definitivo
**Confermiamo Via Lame 261, Castel Maggiore o Via Costituzione 19, Bologna?**
- Conflict tra sito ufficiale e Reteimprese
- Va allineato ovunque (sito + GMB + Reteimprese + LinkedIn + ogni LP)

→ **Decision impact:** local SEO + GMB ranking · risolve audit gap #3

### 5. Foto reali disponibili
**Quanto materiale visivo reale è disponibile oggi?**
- Cantieri (anche anonimizzati)
- Attrezzature in uso (robot, aspiratori, nebulizzatori)
- Ritratto professionale di Alex
- Certificati FGAS / ACCREDIA scansionati

→ **Decision impact:** sostituzione Unsplash hotlinks + credibility · prezzo +/- €600 se devo organizzare shooting

### 6. Stack già attivo
**Cosa esiste già?**
- CRM: GHL / HubSpot / Brevo / nessuno?
- Automation: n8n / Make / Zapier / nessuno?
- Call tracking: CallRail / Aircall / nessuno?
- Analytics: Google Search Console + GA4 collegati / Plausible / nessuno?

→ **Decision impact:** budget tooling mensile · build vs adattamento · prezzo +/- €1.200 setup

### 7. Espansione 12 mesi
**Resta provincia di Bologna o puntate Modena/Ferrara/Imola con LP localizzate?**
- Local-first vs regional-rollout
- GBP satellite (eventuali secondi listing fisici)

→ **Decision impact:** numero di LP da costruire (6 settori × 1 città vs 6 × 4 = 24 LP) · prezzo Phase 2 +€2.800-4.200

### EXTRA · pricing lever
**Vuole rivitalizzare il blog WordPress (2 articoli/mese, pillar SEO + long-tail AEO) o concentrare tutto su LP + Ads + GMB nei primi 90 giorni?**

→ **Decision impact:** retainer mensile da +€600/mese se blog incluso · ROI SEO 6+ mesi vs Ads ROI 30 giorni

---

## 3. Pre-send checklist · 12 punti

- [ ] **#1 SUBSTITUTE** `REPLACE_WITH_WEB3FORMS_KEY` (5 occorrenze in `index.html`) con vero access key Web3Forms
  - Get key: https://web3forms.com/ → genera per progetto Ariapura
  - Trova/sostituisci globale 5 volte
- [ ] **#2 GIT INIT + PUSH**
  - `cd C:\Users\info\OneDrive\Desktop\GITHUB\skynetlabs-ariapura-cinema`
  - `git init && git add -A && git commit -m "Initial cinema bundle: 5 cinematic variants for Ariapura speculative pitch"`
  - `gh repo create waseemnasir2k26/skynetlabs-ariapura-cinema --public --source=. --remote=origin --push`
- [ ] **#3 VERCEL DEPLOY**
  - `vercel --prod` (oppure import via dashboard)
  - Verify URL `https://skynetlabs-ariapura-cinema.vercel.app` ritorna 200
- [ ] **#4 SMOKE TEST INCOGNITO** — apri demo in finestra privata, clicca tutti e 5 i bottoni V1→V5, verifica:
  - Switcher persists tra reload (localStorage)
  - V1 Aether: particle field renderizza (Three.js carica)
  - V2 Solomeo: Ken-Burns CSS animation parte
  - V3 Cleanroom: layout monospace ok
  - V4 Terra Nuova: parallax fog scroll funziona
  - V5 Cinecittà: letterbox 2.39:1 visibile
- [ ] **#5 FORM SMOKE TEST** — submit form di test su 1 variant per verificare email ricezione Web3Forms
- [ ] **#6 MOBILE 320PX** — DevTools responsive, verifica nessun overflow orizzontale
- [ ] **#7 LIGHTHOUSE V1** — V1 Aether è il più pesante (Three.js). Verifica LCP <3s su 4G simulato. Se fallisce, lazy-load il canvas o disable Three.js auto-init
- [ ] **#8 SCHEMA VALIDATION** — incolla JSON-LD in https://validator.schema.org/ → 0 errori
- [ ] **#9 LANG + DIRECTION** — verifica `<html lang="it">` (✅ già impostato)
- [ ] **#10 ROBOTS** — verifica `<meta name="robots" content="noindex, nofollow">` ancora attivo (✅ speculative)
  - Verifica `robots.txt` ancora `Disallow: /` (✅)
- [ ] **#11 PITCH EMAIL FINAL CHECK**
  - Aggiungi telefono/WhatsApp/LinkedIn Waseem in firma
  - Testa link demo + repo da email client (no broken links)
  - Verifica subject line non finisca in spam (Gmail test)
- [ ] **#12 SEND**
  - Destinatario: info@ariapura.org
  - Timing: lun-mer 09:30-11:00 italiano
  - Trackable subject: "Ariapura · 5 piste cinematografiche prima di proporLe qualcosa"
  - Save sent copy in CRM/email folder "Ariapura outreach"

---

## 4. Follow-up cadence (post-send)

| Timing | Action | Channel |
|--------|--------|---------|
| T+0 | Send pitch | Email |
| T+24h | Verifica open via tracking pixel (se attivo) | dashboard |
| T+72h | Se silenzio: follow-up #1 con SEMrush screenshot dei competitor che hanno acquisito traffico (Alisea / AirBio) | Email |
| T+5d | Se silenzio: follow-up #2 via LinkedIn (cerca Alex su LI Bologna HVAC) | LinkedIn DM |
| T+10d | Se silenzio: follow-up #3 con un mini-loom di 90s che mostra V2 vs V3 nel browser | Email + Loom |
| T+14d | Mark as cold lead, sposta in nurture sequence GHL "ariapura-cold" | CRM |

---

## 5. What to do once client replies

### Scenario A · Risposta positiva ("mi interessa, parliamone")
1. Schedula call 30min via Cal.com
2. Prepara Phase 1 contract (€2.400-3.200) basato su risposte alle 7 Qs
3. Richiedi material kit (foto reali + P.IVA + cognome + accessi tecnici)
4. Setup ariapura GHL workspace
5. Apri pipeline "Ariapura Phase 1" in CRM SkynetLabs

### Scenario B · Risposta tiepida ("interessante ma costoso/non urgente")
1. Riposta con Phase 1 mini ad ingaggio ridotto (€1.400 fix dei 6 audit gaps soltanto, no LP)
2. Posiziona come "test in 7 giorni, poi decidiamo se continuare"
3. Lock-in in pipeline come MQL (qualified lead, slow burn)

### Scenario C · Risposta negativa o silenzio T+14d
1. Sposta in nurture sequence "Ariapura cold"
2. Newsletter mensile con 1 case study HVAC italiano + 1 audit gap pubblico
3. Riapri annuale con outreach LinkedIn diretto a Alex
4. Repo resta pubblico come case study SkynetLabs (anonymized se necessario)

---

## 6. Risk register pre-send

| Rischio | Probabilità | Mitigazione |
|---------|-------------|-------------|
| Email finisce in spam | Media | Test pre-send Gmail/Outlook · evita link shortener · cita testo nel corpo non solo link |
| Cliente non capisce le 5 variants | Bassa | Lo switcher è on-screen + label chiare V1-V5 + descrizione 1 riga ognuno nel pitch |
| Three.js V1 lag su mobile vecchio | Media | V1 init solo se selezionata · fallback statico da implementare in v2 se feedback negativo |
| Cliente confuso da listino indicativo | Bassa | Disclaimer ripetuto in ogni variant · il "preventivo personalizzato" è chiaro |
| Cliente vuole vedere prezzi finali subito | Alta | Pitch dichiara "Prima di parlarLe di onorario" · le 7 Qs sbloccano il prezzo · gestire in call |
| NAP fix lo fa già un altro fornitore | Bassa | Non è un blocco, lavoreremo con il NAP che il cliente conferma |
| Cognome Alex già visibile altrove | Bassa | Verificare LinkedIn Bologna HVAC pre-send per non far sentire stalker |

---

Documento di lavoro SkynetLabs. Ultima revisione: 2026-05-08.
