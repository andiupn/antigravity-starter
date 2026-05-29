---
name: task-add
description: |
  Tambah task baru ke docs/tasks/BACKLOG.md dengan auto-ID (T-NNNN), project tag, dan status pilihan.
  Trigger when: user minta "tambah task", "task-add", "/task-add", "catat task ini", "parkir task ini", "simpan task untuk nanti", atau mau masukkan pekerjaan ke backlog.
  Do NOT trigger when: task hanya untuk session ini (gunakan TodoWrite), atau task sudah ada di BACKLOG dan hanya perlu update status (edit manual).
tools: [Bash, Read, Edit]
model: flash
color: blue
---

# Task Add Skill

Tambah task baru ke `docs/tasks/BACKLOG.md`.

## Proses

1. **Kumpulkan input** — tanya jika belum ada:
   - **Task** — deskripsi singkat, action-oriented (contoh: "Optimize build pipeline")
   - **Project** — `workspace` | `custom-module` | `config`
   - **Status** — default `todo`; pilihan: `todo` | `parked` | `blocked`
   - **Priority** — default `medium`; pilihan: `high` | `medium` | `low`
   - **Due** — opsional, format `YYYY-MM-DD` atau `-`
   - **Catatan/Menunggu** — wajib jika status `parked` or `blocked`
   
   Boleh batch semua dalam satu pertanyaan jika belum ada.

2. **Generate ID** — baca baris `**Last ID:** T-NNNN` dari BACKLOG.md, increment 1, format 4 digit.

3. **Tentukan section target:**
   - `todo` → section `## Todo`
   - `in-progress` → section `## In Progress`
   - `parked` → section `## Parked`
   - `blocked` → section `## Blocked`

4. **Tambah baris** ke section yang tepat di BACKLOG.md. Format per section:
   - **In Progress / Todo:** `| T-NNNN | <task> | <project> | <priority> | <due> |`
   - **Parked:** `| T-NNNN | <task> | <project> | <priority> | <catatan> |`
   - **Blocked:** `| T-NNNN | <task> | <project> | <priority> | <menunggu> |`
   
   Hapus dummy row `_kosong_` jika masih ada di section target.

5. **Update Last ID** — ganti `**Last ID:** T-XXXX` dengan ID baru.

6. **Verifikasi** — `grep "T-NNNN" docs/tasks/BACKLOG.md`

7. **Report ke user:**
   ```
   ✓ Task ditambahkan:
   
   ID: T-0001
   Task: <deskripsi>
   Project: <project>
   Status: parked
   Priority: high
   
   Lihat: docs/tasks/BACKLOG.md
   ```

## Aturan

- **Jangan** auto-set status `in-progress` kecuali user eksplisit minta
- Jika task ambigu (terlalu umum seperti "update project"), tanya klarifikasi
- Jika user kasih banyak task sekaligus, proses satu per satu, increment ID tiap task
- Kolom "Catatan" untuk Parked wajib diisi — minimal "Akan dilanjutkan setelah X"
- Kolom "Menunggu" untuk Blocked wajib diisi — minimal apa/siapa yang ditunggu
