# Antizwaartekrachtstarter 🛰️

<div align="center">
  <a href="README.md">English</a> | <a href="README.id.md">Bahasa Indonesia</a> | <a href="README.zh.md">简体中文</a> | <a href="README.hi.md">हिन्दी</a> | <a href="README.fr-ca.md">Français (CA)</a> | <a href="README.de.md">Deutsch</a> | <a href="README.fr.md">Français</a> | <a href="README.pt-br.md">Português (BR)</a> | <a href="README.vi.md">Tiếng Việt</a> | <a href="README.pl.md">Polski</a> | <a href="README.ja.md">日本語</a> | <a href="README.ko.md">한국어</a> | <a href="README.es.md">Español</a> | <a href="README.tr.md">Türkçe</a> | <a href="README.it.md">Italiano</a> | <a href="README.ru.md">Русский</a> | <a href="README.uk.md">Українська</a> | <strong>Nederlands</strong> | <a href="README.sv.md">Svenska</a> | <a href="README.ro.md">Română</a>
</div>
<br>

<div align="center">
  <h3><strong>AI-agenten zijn ongelooflijk slim. Maar ze zijn blind in een rommelige werkruimte.</strong></h3>
  <p><strong>Antigravity Starter is een onberispelijke, AI-first Next.js 16-sandbox die uw AI-editors een perfect zicht geeft.</strong></p>

  <p>Stop met het verspillen van tokens, het lijden aan AI-hallucinaties en het worstelen met rommelige mapstructuren. Coderen met AI zou als magie moeten aanvoelen, en nu doet het dat ook.</p>
</div>

> 📦 Gratis sjabloon van **andiupn** ([kuncimu.com](https://kuncimu.com)) · Gelicentieerd onder [MIT-licentie](LICENSE)  
> ☕ Indien nuttig, [koop een kopje koffie voor me](https://ko-fi.com/andiupn) · 🚀 Heb je status-first monorepos voor meerdere projecten nodig? Probeer de [PRO-versie](https://github.com/sponsors/andiupn?frequency=monthly)

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](LICENSE)
[![GitHub release](https://img.shields.io/github/v/release/andiupn/antigravity-starter)](https://github.com/andiupn/antigravity-starter/releases)
[![Ko-Fi](https://img.shields.io/badge/Ko--fi-Support-ff5f5f?logo=ko-fi)](https://ko-fi.com/andiupn)
[![Patreon](https://img.shields.io/badge/Patreon-Support-f96854?logo=patreon)](https://patreon.com/AndiUpn)
[![Trakteer](https://img.shields.io/badge/Trakteer-Support-red?logo=trakteer)](https://trakteer.id/andi_upn/gift)
[![Saweria](https://img.shields.io/badge/Saweria-Support-yellow?logo=saweria)](https://saweria.co/andiupn)

---

## 💡 Het probleem: waarom traditionele werkruimten tekortschieten op het gebied van AI
AI-agenten (Cursor, Gemini, Claude) zijn fenomenaal capabel. Maar als ze in standaard, rommelige mappen worden geplaatst, raken ze verdwaald. Ze lezen irrelevante mappen, blazen je tokenbudget op, hallucineren en plaatsen bestanden in de verkeerde mappen omdat er geen duidelijke grenzen zijn.

---

## ⚡ De oplossing: drie pijlers van premium AI-steigers

### 1. 🛰️ Perfecte visie voor AI (AI-First Layout)
We hebben elke map, configuratie en `.gitignore` regel ontworpen om als routekaarten voor uw AI te fungeren. De werkruimte is extreem schoon, waardoor Cursor of Gemini uw volledige **Next.js 16 + React 19 + Tailwind v4**-architectuur in minder dan 3 seconden kunnen begrijpen. Geen verspilde tokens, maximale nauwkeurigheid.

### 2. 🤖 Gespecialiseerd team, geen generieke chatbot
Je praat niet tegen een lege AI-box. Je krijgt een team van 2 vooraf geconfigureerde, zeer gespecialiseerde en autonome AI-agenten:
- **`@code-reviewer`** — Uw rigoureuze, strikte QA-team dat de codekwaliteit, linten en structuur beoordeelt voordat er commits worden gemaakt.
- **`@research-assistant`** — Een snelle, kosteneffectieve onderzoeksagent die is toegesneden op het veilig verkennen van nieuwe API-documenten en -bibliotheken.

### 3. ⚡ Vaardigheden met één klik (workflows)
Voer complexe ontwikkelingsworkflows uit met eenvoudige opdrachten. Uitgerust met 8 herbruikbare automatiseringsworkflows (`/skills`) die het handmatig opstellen van steigers, omgevingscontrole en het schrijven van tests tot een taak van 1 seconde maken.

---

## 📊 LITE versus PRO: de premium-upgrade

| Wat u kunt doen | 🆓 LITE (gratis) | 💎 PRO (betaald) |
|---|:---:|:---:|
| **Gespecialiseerde agenten** | 2 | 5 (+ planner, architectuur, beveiliging) |
| **Workflowvaardigheden** | 8 | 23 (+ Drizzle-synchronisatie, Docker, regels-audit, etc.) |
| **Werkruimtestructuur** | Eenvoudig (`src/`, `docs/`) | Status-eerste Monorepo (`active/`, `staging/`, etc.) |
| **Ops Ready-configuratie** | ❌ | ✅ (Docker Compose, Caddyfile) |
| **Projectvoorinstellingen** | 1 (Volgende.js) | 4 (Volgende app, SPA, Laravel, Flutter) |

👉 **[Bekijk de volledige functievergelijkings- en upgradehandleiding](COMPARISON.md)**

---

## 📂 Blauwdruk werkruimte

```
your-workspace/
  .gemini/             # AI agent configs, automation skills, and wiki
  docs/                # Pristine research and implementation plans
  src/                 # Main directory for your application source code
  .env.example         # Template for environment variables
  .gitignore           # Standard Git ignore file
  .mcp.json            # Model Context Protocol (MCP) configuration
  GEMINI.md            # AI coding rules & workspace guidelines
  LICENSE              # Project license (MIT License)
```

---

## 🚀 Ga aan de slag in 3 stappen

### 1. Configuraties kopiëren:

```bash
cp .env.example .env
```

*(Voer uw `GITHUB_TOKEN` in om repository-integraties in te schakelen).*

### 2. AI-rechten instellen:

```bash
cp .gemini/settings.local.example.json .gemini/settings.local.json
```

*(verwijder de opmerkingen en stel `permissions` in, afhankelijk van uw besturingssysteem).*

### 3. Begin met coderen:
Open deze werkruimte in uw favoriete AI-vriendelijke editor en ervaar de snelheid.

---

## 💖 Steun dit project (donaties)

Als deze sjabloon uw codeerworkflow heeft versneld, kunt u overwegen het volgende te ondersteunen:
- **Ko-fi:** [ko-fi.com/andiupn](https://ko-fi.com/andiupn)
- **Patreon:** [patreon.com/AndiUpn](https://patreon.com/AndiUpn)
- **Trakteer:** [trakteer.id/andi_upn/gift](https://trakteer.id/andi_upn/gift)
- **Saweria:** [saweria.co/andiupn](https://saweria.co/andiupn)

---

## 📄 Licentie

Dit project is gelicentieerd onder de **MIT-licentie**. Zie het bestand [LICENSE](LICENSE) voor meer informatie.