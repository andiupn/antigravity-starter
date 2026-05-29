---
name: research-new
description: |
  Buat file riset baru di docs/research/ dengan frontmatter pre-filled (ID, tanggal, status, dll).
  Trigger when: user minta "buat riset baru", "research-new", "/research-new", "mulai riset tentang X", "save findings sebagai artifak", atau ingin simpan hasil riset agent ke file.
  Do NOT trigger when: user hanya tanya/minta riset cepat tanpa perlu disimpan (use research-assistant agent saja), atau update riset yang sudah ada (edit langsung).
tools: [Bash, Write, Read, Edit]
model: flash
color: cyan
---

# Research New Skill

Buat file riset baru di `docs/research/` mengikuti standar workspace.

## Proses

1. **Kumpulkan input dari user** — minimal:
   - **Title** (judul riset, satu kalimat)
   - **Pertanyaan utama** (apa yang ingin dijawab)
   - **Tags** (opsional, comma-separated, contoh: `nextjs,performance`)
   - **Project scope** (default `workspace`, atau custom module/path)
   
   Tanya jika belum jelas. Boleh batch dalam satu pertanyaan.

2. **Generate slug** — kebab-case dari title, max 50 char, hilangkan karakter non-alphanum.

3. **Generate ID & date** — jalankan `date '+%Y%m%d'` lalu `date '+%Y-%m-%d'`. ID format: `RES-<YYYYMMDD>-<slug>`.

4. **Cek konflik nama** — `ls docs/research/RES-<date>-<slug>.md 2>/dev/null`. Jika ada, append `-2`, `-3`, dst sampai unique.

5. **Buat file** — gunakan `docs/templates/research.md` sebagai basis. Replace placeholders:
   - `<slug>` → slug yang di-generate
   - `YYYYMMDD` → tanggal compact
   - `YYYY-MM-DD` → tanggal ISO
   - `<judul riset>` → title
   - `<nama-atau-email>` → ambil dari `git config user.email`, fallback ke `developer`
   - `tags: []` → tags user, format YAML list
   - `project: workspace` → scope user
   - Section "Pertanyaan" → isi dengan pertanyaan utama user
   
   Jangan isi section lain — biar user lanjut sendiri.

6. **Update INDEX.md** — append baris ke section "Active" di `docs/research/INDEX.md`.

7. **Verifikasi** — `head -20 docs/research/RES-...md` untuk konfirmasi frontmatter benar.

8. **Report ke user** — tampilkan:
   - Path file yang dibuat (markdown link)
   - ID
   - Reminder: lanjut isi section "Konteks", "Opsi", "Rekomendasi"

## Aturan

- Default `status: draft` — user upgrade manual saat siap
- Tanya konfirmasi jika title >80 char (kemungkinan terlalu panjang)
- Jangan auto-isi konten body — biar user yang reasoning
- Jika user kasih raw research notes (dari research-assistant), append ke section "Opsi yang Dipertimbangkan" sebagai draft, tapi tetap minta user review
