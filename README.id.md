# Antigravity Starter 🛰️

<div align="center">
  <a href="README.md">English</a> | <strong>Bahasa Indonesia</strong> | <a href="README.zh.md">简体中文</a> | <a href="README.hi.md">हिन्दी</a> | <a href="README.fr-ca.md">Français (CA)</a> | <a href="README.de.md">Deutsch</a> | <a href="README.fr.md">Français</a> | <a href="README.pt-br.md">Português (BR)</a> | <a href="README.vi.md">Tiếng Việt</a> | <a href="README.pl.md">Polski</a>
</div>

<br />

<div align="center">
  <h3><strong>AI Agent sangat cerdas. Tapi mereka buta di ruang kerja yang berantakan.</strong></h3>
  <p><strong>Antigravity Starter adalah tempat bermain Next.js 16 ramah-AI yang memberikan asisten AI Anda pandangan sempurna.</strong></p>

  <p>Hentikan pemborosan token, halusinasi AI yang berulang, dan folder yang berantakan. Coding bersama AI seharusnya terasa seperti keajaiban—dan sekarang keajaiban itu nyata.</p>
</div>

> 📦 Free template by **andiupn** ([kuncimu.com](https://kuncimu.com)) · Licensed under [MIT License](LICENSE)  
> ☕ Jika bermanfaat, [beli saya kopi](https://ko-fi.com/andiupn) · 🚀 Butuh monorepo multi-proyek profesional? Coba [versi PRO](https://github.com/sponsors/andiupn?frequency=monthly)

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](LICENSE)
[![GitHub release](https://img.shields.io/github/v/release/andiupn/antigravity-starter)](https://github.com/andiupn/antigravity-starter/releases)
[![Ko-Fi](https://img.shields.io/badge/Ko--fi-Support-ff5f5f?logo=ko-fi)](https://ko-fi.com/andiupn)
[![Patreon](https://img.shields.io/badge/Patreon-Support-f96854?logo=patreon)](https://patreon.com/AndiUpn)
[![Trakteer](https://img.shields.io/badge/Trakteer-Support-red?logo=trakteer)](https://trakteer.id/andi_upn/gift)
[![Saweria](https://img.shields.io/badge/Saweria-Support-yellow?logo=saweria)](https://saweria.co/andiupn)

---

## 💡 Masalahnya: Mengapa Workspace Tradisional Merusak AI
AI Agent (Cursor, Gemini, Claude) memiliki kemampuan luar biasa. Namun saat dilempar ke direktori standar yang berantakan, mereka tersesat. Mereka membaca folder tidak penting, membakar anggaran token Anda, berhalusinasi, dan meletakkan file di tempat yang salah karena tidak adanya batas struktur yang jelas.

---

## ⚡ Solusinya: Tiga Pilar Scaffolding AI Premium

### 1. 🛰️ Pandangan Sempurna untuk AI (Tata Letak Ramah-AI)
Kami merancang setiap folder, konfigurasi, dan aturan `.gitignore` sebagai peta jalan bagi AI. Workspace ini sangat bersih, memungkinkan Cursor atau Gemini memahami seluruh arsitektur **Next.js 16 + React 19 + Tailwind v4** Anda kurang dari 3 detik. Nol token terbuang, akurasi maksimal.

### 2. 🤖 Tim Spesialis, Bukan Chatbot Generik
Anda tidak berbicara dengan kotak obrolan AI biasa yang kosong. Anda mendapatkan tim berisi 2 agen AI yang sangat spesifik dan bekerja secara otonom:
- **`@code-reviewer`** — Tim QA ketat Anda yang meninjau kualitas kode, linting, dan struktur sebelum komit.
- **`@research-assistant`** — Agen riset berkecepatan tinggi dan hemat biaya untuk menjelajahi API baru dan pustaka (libraries) secara aman.

### 3. ⚡ Otomasi Cepat Sekali Klik (Skills)
Jalankan alur kerja pengembangan yang rumit dengan perintah sederhana. Dilengkapi 8 otomasi alur kerja reusable (`/skills`) yang mengubah tugas pembuatan kerangka folder, pengecekan lingkungan, dan penulisan unit test menjadi tugas 1 detik saja.

---

## 📊 LITE vs PRO: Upgrade Premium

| Fitur | 🆓 LITE (Gratis) | 💎 PRO (Berbayar) |
|---|:---:|:---:|
| **Specialized Agents** | 2 | 5 (+ planner, architecture, security) |
| **Workflow Skills** | 8 | 23 (+ Drizzle sync, Docker, rules-audit, dll.) |
| **Struktur Workspace** | Simple (`src/`, `docs/`) | Status-first Monorepo (`active/`, `staging/`, dll.) |
| **Ops Ready Config** | ❌ | ✅ (Docker Compose, Caddyfile) |
| **Project Presets** | 1 (Next.js) | 4 (Next App, SPA, Laravel, Flutter) |

👉 **[Lihat Perbandingan Fitur Lengkap & Cara Upgrade](COMPARISON.md)**

---

## 📂 Struktur Repositori

```
your-workspace/
  .gemini/             # Konfigurasi agen AI, otomasi skills, dan wiki
  docs/                # Tempat menyimpan riset dan rencana implementasi
  src/                 # Direktori utama kode sumber aplikasi Anda
  .env.example         # Templat variabel lingkungan proyek
  .gitignore           # Berkas abaikan Git standar
  .mcp.json            # Konfigurasi Model Context Protocol (MCP)
  GEMINI.md            # Aturan pengodean AI & panduan workspace
  LICENSE              # Lisensi proyek (MIT License)
```

---

## 🚀 Mulai Cepat dalam 3 Langkah

### 1. Salin konfigurasi lingkungan:
```bash
cp .env.example .env
```
*(Isi token autentikasi GitHub Anda di variabel `GITHUB_TOKEN` jika ingin mengaktifkan integrasi repositori).*

### 2. Aktifkan izin AI Agent:
```bash
cp .gemini/settings.local.example.json .gemini/settings.local.json
```
*(Sesuaikan dengan sistem operasi Anda dan buka kunci perizinan).*

### 3. Mulai Coding:
Buka folder ini di editor ramah-AI favorit Anda, dan rasakan kecepatan pengodean sesungguhnya!

---

## 💖 Dukung Proyek Ini (Donasi)

Jika templat starter ini membantu mempercepat alur kerja pengodean Anda, pertimbangkan untuk memberikan dukungan:
- **Ko-fi:** [ko-fi.com/andiupn](https://ko-fi.com/andiupn)
- **Patreon:** [patreon.com/AndiUpn](https://patreon.com/AndiUpn)
- **Trakteer (Indonesia):** [trakteer.id/andi_upn/gift](https://trakteer.id/andi_upn/gift)
- **Saweria (Indonesia):** [saweria.co/andiupn](https://saweria.co/andiupn)

---

## 📄 Lisensi

Proyek ini dilisensikan di bawah **MIT License**. Lihat berkas [LICENSE](LICENSE) untuk informasi lebih lanjut.
