# Démarreur antigravité 🛰️

<div align="center">
  <a href="README.md">English</a> | <a href="README.id.md">Bahasa Indonesia</a> | <a href="README.zh.md">简体中文</a> | <a href="README.hi.md">हिन्दी</a> | <a href="README.fr-ca.md">Français (CA)</a> | <a href="README.de.md">Deutsch</a> | <strong>Français</strong> | <a href="README.pt-br.md">Português (BR)</a> | <a href="README.vi.md">Tiếng Việt</a> | <a href="README.pl.md">Polski</a> | <a href="README.ja.md">日本語</a> | <a href="README.ko.md">한국어</a> | <a href="README.es.md">Español</a> | <a href="README.tr.md">Türkçe</a> | <a href="README.it.md">Italiano</a> | <a href="README.ru.md">Русский</a> | <a href="README.uk.md">Українська</a> | <a href="README.nl.md">Nederlands</a> | <a href="README.sv.md">Svenska</a> | <a href="README.ro.md">Română</a>
</div>

<br />

<div align="center">
  <h3><strong>Les agents AI sont incroyablement intelligents. Mais ils sont aveugles dans un espace de travail en désordre.</strong></h3>
  <p><strong>Antigravity Starter est un bac à sable Next.js 16 immaculé et axé sur l'IA qui donne à vos éditeurs d'IA une vision parfaite.</strong></p>

  <p>Arrêtez de gaspiller des jetons, de souffrir d'hallucinations de l'IA et de lutter avec des structures de dossiers désordonnées. Coder avec l'IA devrait ressembler à de la magie, et c'est désormais le cas.</p>
</div>

> 📦 Modèle gratuit par **andiupn** ([kuncimu.com](https://kuncimu.com)) · Sous licence [Licence MIT](LICENSE)  
> ☕ Si utile, [achetez-moi un café](https://ko-fi.com/andiupn) · 🚀 Besoin de monorepos multi-projets axés sur le statut ? Essayez la [version PRO](https://github.com/sponsors/andiupn?frequency=monthly)

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](LICENSE)
[![GitHub release](https://img.shields.io/github/v/release/andiupn/antigravity-starter)](https://github.com/andiupn/antigravity-starter/releases)
[![Ko-Fi](https://img.shields.io/badge/Ko--fi-Support-ff5f5f?logo=ko-fi)](https://ko-fi.com/andiupn)
[![Patreon](https://img.shields.io/badge/Patreon-Support-f96854?logo=patreon)](https://patreon.com/AndiUpn)
[![Trakteer](https://img.shields.io/badge/Trakteer-Support-red?logo=trakteer)](https://trakteer.id/andi_upn/gift)
[![Saweria](https://img.shields.io/badge/Saweria-Support-yellow?logo=saweria)](https://saweria.co/andiupn)

---

## 💡 Le problème : pourquoi les espaces de travail traditionnels échouent à l'IA
Les agents IA (Cursor, Gemini, Claude) sont incroyablement capables. Mais lorsqu’ils sont déposés dans des répertoires standard et encombrés, ils se perdent. Ils lisent des dossiers non pertinents, explosent votre budget symbolique, hallucinent et placent les fichiers dans les mauvais répertoires parce qu'il n'y a pas de limites claires.

---

## ⚡ La solution : trois piliers d'un échafaudage d'IA haut de gamme

### 1. 🛰️ Vision parfaite pour l'IA (AI-First Layout)
Nous avons conçu chaque dossier, configuration et règle `.gitignore` pour servir de feuilles de route pour votre IA. L'espace de travail est extrêmement propre, permettant à Cursor ou Gemini de comprendre l'intégralité de votre architecture **Next.js 16 + React 19 + Tailwind v4** en moins de 3 secondes. Zéro jeton gaspillé, précision maximale.

### 2. 🤖 Équipe spécialisée, pas un chatbot générique
Vous ne parlez pas à une boîte IA vide. Vous bénéficiez d'une équipe de 2 agents IA préconfigurés, hautement spécialisés et autonomes :
- **`@code-reviewer`** — Votre équipe d'assurance qualité rigoureuse et stricte qui examine la qualité du code, les peluches et la structure avant la validation.
- **`@research-assistant`** — Un agent de recherche rapide et rentable conçu pour explorer de nouveaux documents et bibliothèques API en toute sécurité.

### 3. ⚡ Compétences en un clic (flux de travail)
Exécutez des workflows de développement complexes avec des commandes simples. Équipé de 8 flux de travail d'automatisation réutilisables (`/skills`) qui transforment l'échafaudage manuel, la vérification de l'environnement et l'écriture de tests en une tâche d'une seconde.

---

## 📊 LITE vs PRO : la mise à niveau Premium

| Ce que vous pouvez faire | 🆓 LITE (Gratuit) | 💎 PRO (Payant) |
|---|:---:|:---:|
| **Agents spécialisés** | 2 | 5 (+ planificateur, architecture, sécurité) |
| **Compétences en matière de flux de travail** | 8 | 23 (+ synchronisation Drizzle, Docker, audit des règles, etc.) |
| **Structure de l'espace de travail** | Simple (`src/`, `docs/`) | Monorepo avec statut premier (`active/`, `staging/`, etc.) |
| **Configuration prête pour les opérations** | ❌ | ✅ (Docker Compose, Caddyfile) |
| **Préréglages du projet** | 1 (Suivant.js) | 4 (Application suivante, SPA, Laravel, Flutter) |

👉 **[Voir la comparaison complète des fonctionnalités et le guide de mise à niveau](COMPARISON.md)**

---

## 📂 Plan d'espace de travail

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

## 🚀 Commencez en 3 étapes

### 1. Copiez les configurations :

```bash
cp .env.example .env
```

*(Insérez votre `GITHUB_TOKEN` pour activer les intégrations de référentiels).*

### 2. Configurez les autorisations de l'IA :

```bash
cp .gemini/settings.local.example.json .gemini/settings.local.json
```

*(Décommentez et définissez `permissions` en fonction de votre système d'exploitation).*

### 3. Commencez à coder :
Ouvrez cet espace de travail dans votre éditeur préféré, compatible avec l'IA, et découvrez la vitesse.

---

## 💖 Soutenez ce projet (Dons)

Si ce modèle a accéléré votre flux de travail de codage, envisagez de prendre en charge :
- **Ko-fi :** [ko-fi.com/andiupn](https://ko-fi.com/andiupn)
- **Patreon :** [patreon.com/AndiUpn](https://patreon.com/AndiUpn)
- **Trakteer :** [trakteer.id/andi_upn/gift](https://trakteer.id/andi_upn/gift)
- **Saweria :** [saweria.co/andiupn](https://saweria.co/andiupn)

---

## 📄 Licence

Ce projet est sous licence **MIT License**. Consultez le fichier [LICENSE](LICENSE) pour plus d'informations.