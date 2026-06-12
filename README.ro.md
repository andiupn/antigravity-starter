# Starter antigravitațional 🛰️

<div align="center">
  <a href="README.md">English</a> | <a href="README.id.md">Bahasa Indonesia</a> | <a href="README.zh.md">简体中文</a> | <a href="README.hi.md">हिन्दी</a> | <a href="README.fr-ca.md">Français (CA)</a> | <a href="README.de.md">Deutsch</a> | <a href="README.fr.md">Français</a> | <a href="README.pt-br.md">Português (BR)</a> | <a href="README.vi.md">Tiếng Việt</a> | <a href="README.pl.md">Polski</a> | <a href="README.ja.md">日本語</a> | <a href="README.ko.md">한국어</a> | <a href="README.es.md">Español</a> | <a href="README.tr.md">Türkçe</a> | <a href="README.it.md">Italiano</a> | <a href="README.ru.md">Русский</a> | <a href="README.uk.md">Українська</a> | <a href="README.nl.md">Nederlands</a> | <a href="README.sv.md">Svenska</a> | <strong>Română</strong>
</div>

<br />

<div align="center">
  <h3><strong>Agenții AI sunt incredibil de inteligenți. Dar sunt orbi într-un spațiu de lucru dezordonat.</strong></h3>
  <p><strong>Antigravity Starter este o cutie de testare Next.js 16 impecabilă, în primul rând AI, care oferă editorilor dumneavoastră AI o viziune perfectă.</strong></p>

  <p>Nu mai irosești jetoane, nu suferi de halucinații AI și nu te mai lupta cu structurile de foldere dezordonate. Codarea cu inteligența artificială ar trebui să pară o magie – și acum este.</p>
</div>

> 📦 Șablon gratuit de la **andiupn** ([kuncimu.com](https://kuncimu.com)) · Licențiat sub [Licență MIT](LICENSE)  
> ☕ Dacă este util, [cumpără-mi o cafea](https://ko-fi.com/andiupn) · 🚀 Ai nevoie de monorepos cu mai multe proiecte pentru status-first? Încercați [versiunea PRO](https://github.com/sponsors/andiupn?frequency=monthly)

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](LICENSE)
[![GitHub release](https://img.shields.io/github/v/release/andiupn/antigravity-starter)](https://github.com/andiupn/antigravity-starter/releases)
[![Ko-Fi](https://img.shields.io/badge/Ko--fi-Support-ff5f5f?logo=ko-fi)](https://ko-fi.com/andiupn)
[![Patreon](https://img.shields.io/badge/Patreon-Support-f96854?logo=patreon)](https://patreon.com/AndiUpn)
[![Trakteer](https://img.shields.io/badge/Trakteer-Support-red?logo=trakteer)](https://trakteer.id/andi_upn/gift)
[![Saweria](https://img.shields.io/badge/Saweria-Support-yellow?logo=saweria)](https://saweria.co/andiupn)

---

## 💡 Problema: De ce spațiile de lucru tradiționale eșuează AI
Agenții AI (Cursor, Gemeni, Claude) sunt extraordinar de capabili. Dar când sunt aruncate în directoare standard, aglomerate, se pierd. Ei citesc foldere irelevante, vă scapă bugetul de simboluri, halucinează și plasează fișiere în directoare greșite, deoarece nu există limite clare.

---

## ⚡ Soluția: Trei piloni ai schelei premium AI

### 1. 🛰️ Viziunea perfectă pentru AI (AI-First Layout)
Am conceput fiecare folder, configurație și regulă `.gitignore` pentru a acționa ca foi de parcurs pentru AI-ul tău. Spațiul de lucru este extrem de curat, permițând lui Cursor sau Gemini să vă înțeleagă întreaga arhitectură **Next.js 16 + React 19 + Tailwind v4** în mai puțin de 3 secunde. Zero jetoane risipite, precizie maximă.

### 2. 🤖 Echipa specializată, nu un Chatbot generic
Nu vorbești cu o cutie AI goală. Obțineți o echipă de 2 agenți AI preconfigurați, foarte specializați și autonomi:
- **`@code-reviewer`** — Echipa ta riguroasă și strictă de control al calității care examinează calitatea codului, scame și structura înainte de comitere.
- **`@research-assistant`** — Un agent de cercetare de mare viteză, rentabil, adaptat pentru a explora în siguranță noile documente și biblioteci API.

### 3. ⚡ Abilități cu un singur clic (fluxuri de lucru)
Executați fluxuri de lucru complexe de dezvoltare cu comenzi simple. Echipat cu 8 fluxuri de lucru de automatizare reutilizabile (`/skills`) care transformă schelele manuale, verificarea mediului și scrierea testelor într-o sarcină de 1 secundă.

---

## 📊 LITE vs PRO: Upgrade Premium

| Ce poți face | 🆓 LITE (gratuit) | 💎 PRO (Plătit) |
|---|:---:|:---:|
| **Agenți de specialitate** | 2 | 5 (+ planificator, arhitectura, securitate) |
| **Abilități de flux de lucru** | 8 | 23 (+ Drizzle sync, Docker, reguli-audit etc.) |
| **Structura spațiului de lucru** | Simplu (`src/`, `docs/`) | Status-primul Monorepo (`active/`, `staging/` etc.) |
| **Configurație Ops Ready** | ❌ | ✅ (Docker Compose, Caddyfile) |
| **Presetări de proiect** | 1 (Next.js) | 4 (Aplicația următoare, SPA, Laravel, Flutter) |

👉 **[Vedeți Ghidul complet de comparare și actualizare a funcțiilor](COMPARISON.md)**

---

## 📂 Planul spațiului de lucru

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

## 🚀 Începeți în 3 pași

### 1. Copiați configurațiile:

```bash
cp .env.example .env
```

*(Introduceți `GITHUB_TOKEN` pentru a activa integrările în depozit).*

### 2. Configurați permisiunile AI:

```bash
cp .gemini/settings.local.example.json .gemini/settings.local.json
```

*(Anulați comentariile și setați `permissions` în funcție de sistemul dvs. de operare).*

### 3. Începeți codarea:
Deschideți acest spațiu de lucru în editorul dvs. favorit prietenos cu AI și experimentați viteza.

---

## 💖 Sprijină acest proiect (donații)

Dacă acest șablon a accelerat fluxul de lucru de codare, luați în considerare sprijinul:
- **Ko-fi:** [ko-fi.com/andiupn](https://ko-fi.com/andiupn)
- **Patreon:** [patreon.com/AndiUpn](https://patreon.com/AndiUpn)
- **Trakteer:** [trakteer.id/andi_upn/gift](https://trakteer.id/andi_upn/gift)
- **Saweria:** [saweria.co/andiupn](https://saweria.co/andiupn)

---

## 📄 Licență

Acest proiect este licențiat sub **Licența MIT**. Consultați fișierul [LICENSE](LICENSE) pentru mai multe informații.