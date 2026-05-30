# Antigravity Starter — Panduan Pengodean & Workspace
<!--
  Scaffolded by Andi UPN (https://github.com/andiupn)
  Official Website & Support: https://kuncimu.com
  Licensed under MIT License
-->

> 📦 Free Template by **Andi UPN** ([kuncimu.com](https://kuncimu.com)) · Licensed under [MIT License](LICENSE)

Workspace terstruktur untuk proyek tunggal (Single-Project) yang dioptimalkan untuk pemula, hobi, dan pengembang solo (*solo developer*) yang berkolaborasi dengan Asisten AI.

**Stack Utama (2026):** Next.js 16 + React 19 + TypeScript + Tailwind v4 + Drizzle ORM + Zod + SQLite  
**Dev Environment:** Multi-OS capable (Linux, macOS, Windows/WSL)

---

## 📂 Struktur Direktori

```
.gemini/
  agents/              # Agen AI spesialis (code-reviewer & research-assistant)
  skills/              # Otomasi alur kerja reusable
  wiki/                # Wiki pengetahuan proyek (README.md & web-tech-2026.md)
  settings.json        # Izin AI Agent global (dilacak oleh Git)
  settings.local.json  # Izin AI Agent lokal (diabaikan oleh Git)
.mcp.json              # Konfigurasi server MCP (GitHub & Filesystem)
.env.example           # Templat variabel lingkungan proyek
GEMINI.md              # Aturan dan panduan workspace ini
README.md              # Dokumentasi umum dan selamat datang
src/                   # Direktori utama kode sumber proyek
docs/
  research/            # Riset eksplorasi — RES-YYYYMMDD-<slug>.md
  plans/               # Rencana implementasi — PLAN-YYYYMMDD-<slug>.md
  templates/           # Templat untuk riset dan rencana
```

---

## 🛠️ Standar Teknologi & Konvensi (Web Tech 2026)

### 1. Web (Next.js 16 + React 19)
- **Framework:** Next.js 16 (App Router). Gunakan Server Components (RSC) secara default untuk kejelasan rute dan rendering data.
- **TypeScript:** Strict mode wajib aktif. **Dilarang menggunakan tipe `any`**. Gunakan interface atau tipe data yang jelas agar AI Agent dapat melakukan analisis dengan presisi tinggi.
- **ORM:** Drizzle ORM (SQL-transparent). Semua perubahan skema wajib melalui migrasi terstruktur (`drizzle-kit generate/push`).
- **Validasi:** Gunakan **Zod** untuk memvalidasi setiap boundary data (props komponen, payload API, dan interaksi database).
- **Styling:** Tailwind CSS v4. Hindari berkas konfigurasi legacy (`tailwind.config.ts/js`); gunakan direktif CSS murni `@theme` dan `@plugin` sesuai standar Tailwind v4.

### 2. JavaScript / TypeScript
- Gunakan ESM Native (`import/export`).
- Utamakan `const` untuk semua variabel, gunakan `let` jika nilainya berubah. Dilarang keras menggunakan `var`.

### 3. Shell Scripts
- Selalu gunakan shebang header: `#!/usr/bin/env bash` dengan opsi pengaman `set -euo pipefail`.
- **CRITICAL:** Skrip shell (`.sh`) wajib menggunakan line endings **LF**. Penggunaan CRLF akan merusak eksekusi di Linux.

---

## 🤖 Aturan Perilaku AI Agent (Universal Rules)

### 1. Protokol Analisis Kode (Forced Reasoning)
Sebelum menulis kode baru, memodifikasi berkas penting, atau menjalankan perintah terminal yang mengubah sistem, Anda **WAJIB** merumuskan analisis singkat berikut:
1. **What:** Masalah atau tugas apa yang ingin diselesaikan?
2. **Why:** Mengapa pendekatan ini merupakan solusi terbaik?
3. **What Risks:** Apa risiko potensial atau efek sampingnya?

### 2. Komunikasi & Bahasa
- Respons wajib disampaikan dalam **Bahasa Indonesia** yang profesional dan ramah, kecuali istilah teknis yang lebih tepat ditulis dalam Bahasa Inggris.
- Hindari kata-kata superlatif yang berlebihan. Sampaikan progres kerja secara faktual dan objektif.

### 3. Batasan Otonomi (Safe Zone)
- **Bebas Mengedit:** AI Agent bebas mengedit dan membuat berkas di dalam `./src`, `./docs`, dan `.gemini/` sesuai instruksi tugas.
- **Dilarang Menghapus:** Jangan pernah menghapus direktori root proyek atau dokumentasi penting tanpa konfirmasi eksplisit dari pengguna.
- **Git Push:** AI Agent diperbolehkan melakukan komit lokal setelah kode lulus uji coba, tetapi keputusan untuk melakukan `git push` ke remote repositori harus diinisiasi oleh pengguna.

---

## 📈 Pengelolaan Konteks & Token

Manfaatkan jendela konteks Gemini yang besar secara efisien:
- Gunakan perintah `/context-handoff` sebelum melakukan `/compact` untuk menyimpan ringkasan progres ke `.gemini/memory/`.
- Gunakan agen spesialis `@research-assistant` untuk riset dan `@code-reviewer` untuk meninjau kualitas kode guna menghemat token sesi utama.

---

## 🗺️ Peta Navigasi Cepat

| Ingin melakukan... | Tujuan Berkas... |
|---|---|
| Memahami repositori starter ini | [README.md](README.md) |
| Menggunakan Agen AI spesialis | [.gemini/AGENTS.md](.gemini/AGENTS.md) |
| Menggunakan keterampilan otomasi | [.gemini/SKILLS.md](.gemini/SKILLS.md) |
| Mengonfigurasi izin AI Agent | [.gemini/SETTINGS.md](.gemini/SETTINGS.md) |
| Mengisi token lingkungan | [.env.example](.env.example) |
| Melihat templat riset & rencana | [docs/templates/](docs/templates/) |
| Membaca standar web 2026 | [.gemini/wiki/patterns/web-tech-2026.md](.gemini/wiki/patterns/web-tech-2026.md) |
