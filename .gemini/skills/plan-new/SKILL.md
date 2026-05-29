---
name: plan-new
description: |
  Buat file plan implementasi baru di docs/plans/ dengan frontmatter pre-filled (ID, tanggal, status, dll).
  Trigger when: user minta "buat plan baru", "plan-new", "/plan-new", "rancang implementasi X", "save plan ini sebagai artifak", atau output dari Plan mode agent yang perlu di-persist.
  Do NOT trigger when: task trivial yang cukup TodoWrite, eksperimen kecil (use experiment-scaffold), riset eksplorasi (use research-new), atau update plan yang sudah ada.
tools: [Bash, Write, Read, Edit]
model: flash
color: green
---

# Plan New Skill

Buat file plan implementasi baru di `docs/plans/` mengikuti standar workspace.

## Proses

### Step 0: Cek apakah butuh deep planning dulu

Sebelum membuat file plan, tanyakan (atau deteksi dari context):
- Apakah plan ini membutuhkan **architectural reasoning** (multi-module, banyak trade-off, keputusan jangka panjang)?

Jika YA dan user belum punya draft reasoning → sarankan:
```
💡 Untuk planning kompleks, gunakan @planner dulu untuk deep thinking,
   lalu pipe outputnya ke sini: /plan-new
```

Jika user sudah punya draft / task sederhana → lanjut langsung ke Step 1.

1. **Kumpulkan input dari user** — minimal:
   - **Title** (judul plan)
   - **Tujuan** (outcome yang dituju, satu kalimat)
   - **Tags** (opsional)
   - **Project scope** (default `workspace`, atau custom module/path)
   - **Riset terkait** (opsional, ID seperti `RES-20260507-...`)
   
   Tanya jika belum jelas.

2. **Generate slug** — kebab-case dari title, max 50 char.

3. **Generate ID & date** — `date '+%Y%m%d'` dan `date '+%Y-%m-%d'`. ID: `PLAN-<YYYYMMDD>-<slug>`.

4. **Cek konflik** — `ls docs/plans/PLAN-<date>-<slug>.md 2>/dev/null`. Jika ada, append `-2`, dst.

5. **Buat file** — basis `docs/templates/plan.md`. Replace placeholders sama seperti research-new. Tambahan:
   - Section "Tujuan" → isi dari user
   - Field `related` → isi ID riset jika ada
   
   Section lain biar user yang isi.

6. **Update INDEX.md** — append baris ke section "Active" di `docs/plans/INDEX.md`.

7. **Verifikasi** — `head -20 docs/plans/PLAN-...md`.

8. **Report ke user** — tampilkan path, ID, dan reminder isi:
   - Scope (in/out)
   - Pendekatan
   - Tahapan implementasi
   - Risiko & mitigasi
   - Kriteria selesai
   - Rollback plan

## Aturan

- Default `status: draft` — user upgrade ke `active` saat plan disetujui & siap dieksekusi
- Jika ada PLAN sebelumnya yang akan di-supersede, isi field `supersedes` dan update PLAN lama dengan `superseded_by` + status `superseded`
