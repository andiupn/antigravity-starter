# 📐 UNIVERSAL CODING STANDARDS
**Scope:** Universal (Shared Core)

---

## 💻 BAHASA PEMROGRAMAN & KONVENSI

### JavaScript & TypeScript
- **ESM Native:** Gunakan ESM imports (`import/export`) secara eksklusif. Hindari `require`/CommonJS kecuali sangat terpaksa.
- **Deklarasi Variabel:** Utamakan `const` untuk semua variabel, gunakan `let` jika nilainya berubah. Dilarang keras menggunakan `var`.
- **Strict TypeScript:** Strict mode wajib aktif. **Dilarang menggunakan tipe `any`**. Setiap data wajib memiliki interface atau type yang eksplisit dan jelas untuk mempermudah analisis agen AI.
- **Validasi Boundary:** Gunakan **Zod** untuk validasi skema di setiap batas lalu lintas data (props, payload API, pembacaan database, masukan pengguna).

### Shell Scripts & Powershell
- **Shebang Header:** Gunakan `#!/usr/bin/env bash` dengan setelan pengaman `set -euo pipefail`.
- **Line Endings:** Semua skrip shell (`.sh`) wajib menggunakan line-ending **LF** (Unix style). CRLF dari Windows akan merusak eksekusi di Linux.
- **Windows Scripts:** Gunakan PowerShell (`.ps1`) untuk skrip baru Windows, jangan gunakan CMD (`.bat`).

---

## 🧹 INTEGRITAS & KERAPIAN KODE

- **Targeted Diffs:** Jaga agar perubahan kode sefokus mungkin. Hanya edit bagian yang relevan dengan tugas. Refactoring massal wajib mendapat persetujuan terlebih dahulu.
- **Preservasi Komentar:** Selalu pertahankan komentar dan *docstrings* bawaan yang tidak berhubungan dengan perubahan Anda. Jangan menghapus dokumentasi asli.
- **Dokumentasikan WHY, bukan WHAT:** Saat menulis komentar baru, jelaskan alasan logis di balik keputusan tersebut (*WHY*), bukan sekadar menjelaskan baris kodingan tersebut melakukan apa (*WHAT*).
- **Tanpa Placeholder:** Jangan membuat implementasi setengah matang (*simple MVP*) atau menuliskan komentar seperti `// TODO: implement later`. Semua kode yang dihasilkan harus fungsional dan siap pakai.
