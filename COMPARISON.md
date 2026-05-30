# LITE vs PRO Comparison — AntiGravity Edition

> Bingung memilih versi mana? Berikut perbandingan fitur lengkap antara edisi LITE (Starter) dan PRO (Premium Workspace).

## TL;DR

- **LITE / Starter (Gratis):** Cocok untuk single-project sederhana. Menyertakan 2 agents utama, 8 universal skills, lisensi open-source MIT, dan struktur proyek standar.
- **PRO / Premium (Berbayar $1–$5):** Ditujukan untuk pengembang serius, freelancer, dan agensi. Menyertakan 5 spesialis agents, 23 skills otomasi universal, docker/caddy ops setup, multi-project status-first workspace, dan 4 preset proyek.

---

## Feature Matrix

| Fitur | 🆓 LITE (Starter) | 💎 PRO (Premium) |
|---|:---:|:---:|
| **Specialized Agents** | 2 | 5 |
| `@code-reviewer` | ✅ | ✅ (Gemini 3.5 Flash + 8K thinking) |
| `@research-assistant` | ✅ | ✅ (Gemini 3.5 Flash) |
| `@architecture-reviewer` | ❌ | ✅ (Gemini 3.5 Flash + 16K thinking) |
| `@planner` (architectural planner) | ❌ | ✅ (Gemini 3.5 Flash + 32K thinking) |
| `@security-reviewer` (OWASP security) | ❌ | ✅ (Gemini 3.5 Flash + 16K thinking) |
| | | |
| **Workflow Skills** | 8 | 23 |
| `/git-workflow` (structured commits) | ✅ | ✅ |
| `/experiment-scaffold` | ✅ | ✅ |
| `/test-writer` | ✅ | ✅ |
| `/validate-agent-config` | ✅ | ✅ |
| `/context-handoff` | ✅ | ✅ |
| `/rules-sync` (sinkronisasi aturan) | ✅ | ✅ |
| `/init-project` | ✅ (Next.js) | ✅ (Semua Preset) |
| `/rules-maintenance` (audit AI rules) | ❌ | ✅ |
| `/database-sync` (Drizzle Kit migration)| ❌ | ✅ |
| `/ops-reload` (Caddy/Docker reloader) | ❌ | ✅ |
| `/knowledge-extract` (harvest session) | ❌ | ✅ |
| `/knowledge-harvest` (cross-project) | ❌ | ✅ |
| `/ui-test` (Chrome DevTools smoke test)| ❌ | ✅ |
| *Dan 10 skills otomasi premium lainnya*| ❌ | ✅ |
| | | |
| **Project Presets (`/init-project`)** | 1 | 4 |
| `nextjs-app` (Next.js 16 App Router) | ✅ | ✅ |
| `nextjs-spa` (Single Page App) | ❌ | ✅ |
| `laravel-inertia` (PHP + React) | ❌ | ✅ |
| `flutter-clean` (Flutter Dart Clean) | ❌ | ✅ |
| | | |
| **Struktur Workspace** | Simple (`src/`, `docs/`) | Status-first Monorepo (`active/`, `staging/`, `archive/`, `shared/`, `ops/`, `artifacts/`) |
| Multi-project orchestration | ❌ | ✅ |
| Project lifecycle workflow | ❌ | ✅ |
| | | |
| **Ops & Docker Config (`ops/`)** | ❌ | ✅ |
| `docker-compose.yml` local stack | ❌ | ✅ |
| `Caddyfile` reverse proxy config | ❌ | ✅ |
| Automated startup scripts | ❌ | ✅ |
| | | |
| **Lisensi & Dukungan** | MIT License | Proprietary Commercial |
| Redistribution allowed | ✅ | ❌ |
| Komersial (proyek klien & internal) | ✅ | ✅ |
| Dukungan Email | Best-effort (Komunitas) | Best-effort (No SLA - Prioritas Tinggi) |
| Pembaruan Berkelanjutan | Via GitHub | Via kuncimu.com |

---

## When to Choose Which?

### Pilih **LITE (Starter)** jika:
- ✅ Anda baru mulai mempelajari orkestrasi AI Agent.
- ✅ Proyek Anda adalah single-project sederhana (1 aplikasi saja).
- ✅ Anda ingin berkontribusi secara open-source atau membuat fork komunitas.
- ✅ Anda ingin mencoba sistem kerja secara gratis terlebih dahulu.

### Pilih **PRO (Premium)** jika:
- ✅ Anda mengelola banyak proyek aktif untuk klien atau internal (Agensi / Freelancer).
- ✅ Anda membutuhkan stack ops Docker & Caddy siap pakai.
- ✅ Anda membutuhkan state-management pengetahuan (Riset, Rencana, ADR) yang terintegrasi.
- ✅ Anda ingin meningkatkan kecepatan pengerjaan dengan 23 skills otomasi yang super lengkap.
- ✅ Anda ingin mendukung pemeliharaan berkelanjutan dari proyek ini.

---

## Upgrade Path

Jika Anda sudah menggunakan versi LITE dan ingin beralih ke PRO:

1. Dapatkan lisensi resmi versi PRO di **[kuncimu.com](https://kuncimu.com)**.
2. Unduh berkas repositori `antigravity-pro`.
3. Pindahkan berkas kode proyek Anda yang sudah ada dari `src/` versi Starter ke direktori `active/web/<nama-proyek>` di versi PRO.
4. Sesuaikan konfigurasi file `GEMINI.md` Anda.

Tidak ada lock-in — Anda dapat kembali ke versi LITE kapan saja secara bebas.

---

## Hubungi Kami

- **Pertanyaan Umum / Masalah:** Silakan buat Issue di GitHub [github.com/andiupn](https://github.com/andiupn).
- **Pertanyaan Pra-Penjualan PRO:** Hubungi kami melalui email di **andi.upn@gmail.com**.

👉 **[Dapatkan Edisi PRO di kuncimu.com](https://kuncimu.com)**
