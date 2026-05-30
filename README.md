# Antigravity Starter 🚀

**Template starter ringan dan ramah AI untuk proyek tunggal (Single-Project).**

> 📦 Free template by **andiupn** ([kuncimu.com](https://kuncimu.com)) · Licensed under [MIT License](LICENSE)
> ☕ If useful, [buy me a coffee](https://ko-fi.com/andiupn) · 🚀 Need more features? Try [PRO version](https://kuncimu.com)

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](LICENSE)
[![Ko-Fi](https://img.shields.io/badge/Ko--fi-Support-ff5f5f?logo=ko-fi)](https://ko-fi.com/andiupn)
[![Patreon](https://img.shields.io/badge/Patreon-Support-f96854?logo=patreon)](https://patreon.com/AndiUpn)

---

## 🌟 Fitur Utama

- **AI-First Design:** Struktur repositori yang dirancang ramah untuk dibaca, dipahami, dan dikelola oleh AI Agent (seperti Gemini, Cursor, dll.).
- **Specialized Agents:** Dilengkapi dengan 2 agen AI spesialis dasar (`code-reviewer` dan `research-assistant`) di `.gemini/agents/`.
- **Workflow Automation:** Dilengkapi dengan 8 otomasi alur kerja reusable (`/skill-name`) di `.gemini/skills/`.
- **Structured Documentation:** Memiliki folder `docs/` terstandarisasi untuk mendokumentasikan riset (`docs/research/`) dan rencana implementasi (`docs/plans/`).
- **Standard Web 2026 Stack Ready:** Konfigurasi bawaan untuk Next.js 16 + React 19 + TypeScript + Tailwind v4 + Drizzle ORM.

---

## 📊 LITE vs PRO Comparison

| Fitur | 🆓 LITE (Gratis) | 💎 PRO (Berbayar) |
|---|:---:|:---:|
| **Specialized Agents** | 2 | 5 (+ planner, architecture, security) |
| **Workflow Skills** | 8 | 23 (+ Drizzle sync, Docker, rules-audit, dll.) |
| **Struktur Workspace** | Simple (`src/`, `docs/`) | Status-first Monorepo (`active/`, `staging/`, dsb.) |
| **Ops Ready Config** | ❌ | ✅ (Docker Compose, Caddyfile) |
| **Project Presets** | 1 (Next.js) | 4 (Next App, SPA, Laravel, Flutter) |

👉 **[Lihat Perbandingan Fitur Lengkap & Cara Upgrade](COMPARISON.md)**

---

## 📂 Struktur Repositori

```
your-workspace/
  .gemini/             # Konfigurasi agen AI, skills otomasi, dan wiki
  docs/                # Tempat menyimpan riset dan rencana implementasi
  src/                 # Direktori utama kode sumber aplikasi Anda
  .env.example         # Templat variabel lingkungan proyek
  .gitignore           # Berkas abaikan Git standar
  .mcp.json            # Konfigurasi Model Context Protocol (MCP)
  GEMINI.md            # Aturan pengodean AI & panduan workspace
  LICENSE              # Lisensi proyek (MIT License)
```

---

## 🚀 Memulai Proyek Anda

### 1. Prasyarat
Pastikan Anda telah memasang:
- Node.js (versi terbaru 2025/2026 direkomendasikan)
- Git untuk pengelolaan versi
- Penyunting kode (seperti VS Code atau Cursor)

### 2. Salin dan Setup Lingkungan
Salin templat variabel lingkungan proyek Anda:
```bash
cp .env.example .env
```
Buka berkas `.env` dan isi token autentikasi GitHub Anda di variabel `GITHUB_TOKEN` jika Anda ingin mengaktifkan Model Context Protocol (MCP) untuk integrasi repositori.

### 3. Aktifkan Izin Izin AI Agent
Salin templat konfigurasi izin lokal untuk AI Agent:
```bash
cp .gemini/settings.local.example.json .gemini/settings.local.json
```
Buka `.gemini/settings.local.json`, sesuaikan dengan sistem operasi Anda (Linux/Windows), dan ubah kunci `"permissions_LINUX"` atau `"permissions_WINDOWS"` menjadi `"permissions"`.

---

## 💖 Dukung Proyek Ini (Donasi)

Jika templat starter ini membantu mempercepat alur kerja pengodean Anda, Anda dapat memberikan dukungan atau donasi melalui tautan berikut:
- **Ko-fi:** [ko-fi.com/andiupn](https://ko-fi.com/andiupn)
- **Patreon:** [patreon.com/AndiUpn](https://patreon.com/AndiUpn)
- **Trakteer:** [trakteer.id/andi_upn/gift](https://trakteer.id/andi_upn/gift)
- **Saweria:** [saweria.co/andiupn](https://saweria.co/andiupn)

Dukungan Anda sangat berarti bagi pengembangan templat dan integrasi perkakas AI yang lebih baik di masa depan!

---

## 📄 Lisensi

Proyek ini dilisensikan di bawah **MIT License**. Lihat berkas [LICENSE](LICENSE) untuk informasi lebih lanjut.
