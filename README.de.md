# Antigravitationsstarter 🛰️

<div align="center">
  <a href="README.md">English</a> | <a href="README.id.md">Bahasa Indonesia</a> | <a href="README.zh.md">简体中文</a> | <a href="README.hi.md">हिन्दी</a> | <a href="README.fr-ca.md">Français (CA)</a> | <strong>Deutsch</strong> | <a href="README.fr.md">Français</a> | <a href="README.pt-br.md">Português (BR)</a> | <a href="README.vi.md">Tiếng Việt</a> | <a href="README.pl.md">Polski</a> | <a href="README.ja.md">日本語</a> | <a href="README.ko.md">한국어</a> | <a href="README.es.md">Español</a> | <a href="README.tr.md">Türkçe</a> | <a href="README.it.md">Italiano</a> | <a href="README.ru.md">Русский</a> | <a href="README.uk.md">Українська</a> | <a href="README.nl.md">Nederlands</a>
</div>

<br />

<div align="center">
  <h3><strong>KI-Agenten sind unglaublich intelligent. Aber in einem unordentlichen Arbeitsbereich sind sie blind.</strong></h3>
  <p><strong>Antigravity Starter ist eine makellose, KI-orientierte Next.js 16-Sandbox, die Ihren KI-Redakteuren eine perfekte Sicht bietet.</strong></p>

  <p>Verschwenden Sie keine Token mehr, leiden Sie nicht mehr unter KI-Halluzinationen und kämpfen Sie nicht mehr mit unordentlichen Ordnerstrukturen. Codieren mit KI sollte sich wie Magie anfühlen – und jetzt tut es das auch.</p>
</div>

> 📦 Kostenlose Vorlage von **andiupn** ([kuncimu.com](https://kuncimu.com)) · Lizenziert unter [MIT-Lizenz](LICENSE)  
> ☕ Wenn nützlich, [kauf mir einen Kaffee](https://ko-fi.com/andiupn) · 🚀 Benötigen Sie Status-First-Monorepos für mehrere Projekte? Probieren Sie die [PRO-Version](https://github.com/sponsors/andiupn?frequency=monthly) aus.

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](LICENSE)
[![GitHub release](https://img.shields.io/github/v/release/andiupn/antigravity-starter)](https://github.com/andiupn/antigravity-starter/releases)
[![Ko-Fi](https://img.shields.io/badge/Ko--fi-Support-ff5f5f?logo=ko-fi)](https://ko-fi.com/andiupn)
[![Patreon](https://img.shields.io/badge/Patreon-Support-f96854?logo=patreon)](https://patreon.com/AndiUpn)
[![Trakteer](https://img.shields.io/badge/Trakteer-Support-red?logo=trakteer)](https://trakteer.id/andi_upn/gift)
[![Saweria](https://img.shields.io/badge/Saweria-Support-yellow?logo=saweria)](https://saweria.co/andiupn)

---

## 💡 Das Problem: Warum traditionelle Arbeitsbereiche die KI versagen
KI-Agenten (Cursor, Gemini, Claude) sind phänomenal fähig. Aber wenn sie in standardmäßigen, überfüllten Verzeichnissen abgelegt werden, gehen sie verloren. Sie lesen irrelevante Ordner, sprengen Ihr Token-Budget, halluzinieren und legen Dateien in den falschen Verzeichnissen ab, weil es keine klaren Grenzen gibt.

---

## ⚡ Die Lösung: Drei Säulen des Premium-KI-Gerüsts

### 1. 🛰️ Perfekte Vision für KI (AI-First-Layout)
Wir haben jeden Ordner, jede Konfiguration und jede `.gitignore`-Regel so entworfen, dass sie als Roadmaps für Ihre KI dienen. Der Arbeitsbereich ist äußerst übersichtlich, sodass Cursor oder Gemini Ihre gesamte **Next.js 16 + React 19 + Tailwind v4**-Architektur in weniger als 3 Sekunden verstehen können. Keine verschwendeten Token, maximale Genauigkeit.

### 2. 🤖 Spezialisiertes Team, kein generischer Chatbot
Sie sprechen nicht mit einer leeren KI-Box. Sie erhalten ein Team aus 2 vorkonfigurierten, hochspezialisierten und autonomen KI-Agenten:
- **`@code-reviewer`** – Ihr strenges, strenges QA-Team, das Codequalität, Lints und Struktur vor Commits überprüft.
- **`@research-assistant`** – Ein schneller, kostengünstiger Rechercheagent, der darauf zugeschnitten ist, neue API-Dokumente und -Bibliotheken sicher zu erkunden.

### 3. ⚡ One-Click-Skills (Workflows)
Führen Sie komplexe Entwicklungsworkflows mit einfachen Befehlen aus. Ausgestattet mit 8 wiederverwendbaren Automatisierungsworkflows (`/skills`), die manuelles Gerüstbau, Umgebungsprüfung und Testschreiben in eine 1-Sekunden-Aufgabe verwandeln.

---

## 📊 LITE vs. PRO: Das Premium-Upgrade

| Was Sie tun können | 🆓 LITE (Kostenlos) | 💎 PRO (Kostenpflichtig) |
|---|:---:|:---:|
| **Spezialisierte Agenten** | 2 | 5 (+ Planer, Architektur, Sicherheit) |
| **Workflow-Fähigkeiten** | 8 | 23 (+ Drizzle-Synchronisierung, Docker, Regelprüfung usw.) |
| **Arbeitsbereichsstruktur** | Einfach (`src/`, `docs/`) | Status-First-Monorepo (`active/`, `staging/` usw.) |
| **Ops Ready Config** | ❌ | ✅ (Docker Compose, Caddyfile) |
| **Projektvoreinstellungen** | 1 (Next.js) | 4 (Nächste App, SPA, Laravel, Flutter) |

👉 **[Vollständigen Funktionsvergleich und Upgrade-Leitfaden anzeigen](COMPARISON.md)**

---

## 📂 Workspace Blueprint

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

## 🚀 Beginnen Sie in 3 Schritten

### 1. Konfigurationen kopieren:

```bash
cp .env.example .env
```

*(Geben Sie Ihr `GITHUB_TOKEN` ein, um Repository-Integrationen zu aktivieren.*

### 2. AI-Berechtigungen einrichten:

```bash
cp .gemini/settings.local.example.json .gemini/settings.local.json
```

*(Entfernen Sie das Kommentarzeichen und stellen Sie `permissions` entsprechend Ihrem Betriebssystem ein).*

### 3. Beginnen Sie mit dem Codieren:
Öffnen Sie diesen Arbeitsbereich in Ihrem bevorzugten KI-freundlichen Editor und erleben Sie die Geschwindigkeit.

---

## 💖 Unterstützen Sie dieses Projekt (Spenden)

Wenn diese Vorlage Ihren Codierungsworkflow beschleunigt hat, sollten Sie Folgendes unterstützen:
- **Ko-fi:** [ko-fi.com/andiupn](https://ko-fi.com/andiupn)
- **Patreon:** [patreon.com/AndiUpn](https://patreon.com/AndiUpn)
- **Trakteer:** [trakteer.id/andi_upn/gift](https://trakteer.id/andi_upn/gift)
- **Saweria:** [saweria.co/andiupn](https://saweria.co/andiupn)

---

## 📄 Lizenz

Dieses Projekt ist unter der **MIT-Lizenz** lizenziert. Weitere Informationen finden Sie in der Datei [LICENSE](LICENSE).