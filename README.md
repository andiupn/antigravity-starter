# Antigravity Starter 🚀

<div align="center">
  <strong>English</strong> | <a href="README.id.md">Bahasa Indonesia</a>
</div>

<br />

**A lightweight, AI-friendly starter template for single-project workspaces.**

> 📦 Free template by **andiupn** ([kuncimu.com](https://kuncimu.com)) · Licensed under [MIT License](LICENSE)  
> ☕ If useful, [buy me a coffee](https://ko-fi.com/andiupn) · 🚀 Need more features? Try the [PRO version](https://kuncimu.com)

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](LICENSE)
[![GitHub release](https://img.shields.io/github/v/release/andiupn/antigravity-starter)](https://github.com/andiupn/antigravity-starter/releases)
[![Ko-Fi](https://img.shields.io/badge/Ko--fi-Support-ff5f5f?logo=ko-fi)](https://ko-fi.com/andiupn)
[![Patreon](https://img.shields.io/badge/Patreon-Support-f96854?logo=patreon)](https://patreon.com/AndiUpn)
[![Trakteer](https://img.shields.io/badge/Trakteer-Support-red?logo=trakteer)](https://trakteer.id/andi_upn/gift)
[![Saweria](https://img.shields.io/badge/Saweria-Support-yellow?logo=saweria)](https://saweria.co/andiupn)

---

## 🌟 Key Features

- **AI-First Design:** Repository structure optimized to be read, understood, and managed by AI Agents (such as Gemini, Cursor, etc.).
- **Specialized Agents:** Equipped with 2 basic specialized AI agents (`code-reviewer` and `research-assistant`) in `.gemini/agents/`.
- **Workflow Automation:** Includes 8 reusable automation workflows (`/skill-name`) in `.gemini/skills/`.
- **Structured Documentation:** Standardized `docs/` folder for documenting research (`docs/research/`) and implementation plans (`docs/plans/`).
- **Standard Web 2026 Stack Ready:** Pre-configured configurations for Next.js 16 + React 19 + TypeScript + Tailwind CSS v4 + Drizzle ORM.

---

## 📊 LITE vs PRO Comparison

| Feature | 🆓 LITE (Free) | 💎 PRO (Paid) |
|---|:---:|:---:|
| **Specialized Agents** | 2 | 5 (+ planner, architecture, security) |
| **Workflow Skills** | 8 | 23 (+ Drizzle sync, Docker, rules-audit, etc.) |
| **Workspace Structure** | Simple (`src/`, `docs/`) | Status-first Monorepo (`active/`, `staging/`, etc.) |
| **Ops Ready Config** | ❌ | ✅ (Docker Compose, Caddyfile) |
| **Project Presets** | 1 (Next.js) | 4 (Next App, SPA, Laravel, Flutter) |

👉 **[View Full Feature Comparison & Upgrade Guide](COMPARISON.md)**

---

## 📂 Repository Structure

```
your-workspace/
  .gemini/             # AI agent configs, automation skills, and wiki
  docs/                # Place for research and implementation plans
  src/                 # Main directory for your application source code
  .env.example         # Template for environment variables
  .gitignore           # Standard Git ignore file
  .mcp.json            # Model Context Protocol (MCP) configuration
  GEMINI.md            # AI coding rules & workspace guidelines
  LICENSE              # Project license (MIT License)
```

---

## 🚀 Getting Started

### 1. Prerequisites
Make sure you have installed:
- Node.js (latest 2025/2026 version recommended)
- Git for version control
- Code editor (such as VS Code or Cursor)

### 2. Copy and Setup Environment
Copy your project environment variables template:
```bash
cp .env.example .env
```
Open the `.env` file and fill in your GitHub personal access token in the `GITHUB_TOKEN` variable if you want to enable the Model Context Protocol (MCP) for repository integration.

### 3. Enable AI Agent Permissions
Copy the local permission configuration template for the AI Agent:
```bash
cp .gemini/settings.local.example.json .gemini/settings.local.json
```
Open `.gemini/settings.local.json`, adapt it to your operating system (Linux/Windows), and change the `"permissions_LINUX"` or `"permissions_WINDOWS"` key to `"permissions"`.

---

## 💖 Support This Project (Donations)

If this starter template helps speed up your coding workflow, consider supporting or donating via the following links:
- **Ko-fi:** [ko-fi.com/andiupn](https://ko-fi.com/andiupn)
- **Patreon:** [patreon.com/AndiUpn](https://patreon.com/AndiUpn)
- **Trakteer:** [trakteer.id/andi_upn/gift](https://trakteer.id/andi_upn/gift)
- **Saweria:** [saweria.co/andiupn](https://saweria.co/andiupn)

Your support is highly valued and helps us maintain and improve AI template integrations in the future!

---

## 📄 License

This project is licensed under the **MIT License**. See the [LICENSE](LICENSE) file for more information.
