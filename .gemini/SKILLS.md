# Skills: Otomasi Alur Kerja Reusable

Skills adalah **skrip alur kerja terstruktur** yang dijalankan melalui perintah slash (`/nama-skill`) untuk mengotomatiskan tugas-tugas berulang dan memastikan kepatuhan terhadap standar proyek.

## Daftar 8 Skills Utama

Berikut adalah daftar 8 skills bawaan di Antigravity Starter:

| Skill | Perintah | Deskripsi | Kapan Digunakan |
|---|---|---|---|
| **context-handoff** | `/context-handoff` | Menyimpan ringkasan sesi saat ini ke `.gemini/memory/` | Sebelum melakukan *context reset* (`/compact`) atau di akhir sesi panjang. |
| **experiment-scaffold** | `/experiment-scaffold` | Menyiapkan folder eksperimen baru beserta templat README | Saat ingin memulai uji coba fitur baru atau eksperimen terisolasi. |
| **git-workflow** | `/git-workflow` | Mengelola komit Git yang rapi dan penanganan cabang | Sebelum melakukan komit dan dorong (*push*) perubahan ke repositori. |
| **plan-new** | `/plan-new` | Membuat dokumen rencana implementasi baru di `docs/plans/` | Saat merancang arsitektur atau rencana pengerjaan fitur baru. |
| **research-new** | `/research-new` | Membuat dokumen riset teknologi baru di `docs/research/` | Saat mencatat hasil riset library atau eksplorasi teknologi baru. |
| **task-add** | `/task-add` | Menambahkan tugas baru ke daftar backlog proyek | Untuk memarkir ide atau tugas yang akan dikerjakan nanti. |
| **validate-agent-config** | `/validate-agent-config` | Memvalidasi keselarasan konfigurasi agen dan keterampilan | Untuk memverifikasi integritas berkas aturan proyek `.gemini/`. |
| **wiki-lint** | `/wiki-lint` | Memeriksa keutuhan tautan dan berkas di wiki proyek | Untuk memastikan dokumentasi wiki di `.gemini/wiki/` tetap rapi. |

---

## Cara Menjalankan Skill

Ketik perintah slash di awal prompt Anda:
```markdown
/context-handoff
```
```markdown
/experiment-scaffold
Name: routing-optimizations
Description: Menguji performa rute Next.js 16
```
Agent akan mengenali perintah tersebut dan menjalankan alur kerja langkah-demi-langkah sesuai berkas panduan di masing-masing direktori `.gemini/skills/<nama-skill>/SKILL.md`.
