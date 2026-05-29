# 🛡️ DIAGNOSTIK PROAKTIF & PROTOKOL SELF-HEALING
**Scope:** Universal (Shared Core)

---

## 🔍 PRE-TASK CHECKLIST & DIAGNOSTIK

Sebelum memulai pekerjaan besar atau modifikasi sistem:
1. **Validasi OS & Shell:** Verifikasi OS aktif (Linux/macOS vs Windows) dan terminal shell yang berjalan sebelum mempercayai file lingkungan yang tersimpan.
2. **Prediksi Efek Samping:** Secara proaktif perkirakan efek samping dari eksekusi perintah (misal: port tabrakan, konflik dependensi package, atau perubahan hak akses berkas).
3. **Cek Deprecations:** Jangan menggunakan perkakas lama jika ada versi baru yang direkomendasikan.

---

## 🩹 PROTOKOL SELF-HEALING (PEMULIHAN MANDIRI)

Jika terjadi kegagalan eksekusi perintah terminal atau build error:

### Alur Kerja Pemulihan (Maksimal 3 Percobaan)
1. **Analisis Error:** Pindai pesan kesalahan untuk mengidentifikasi apakah kegagalan disebabkan oleh masalah:
   - Hak akses berkas (Permission denied)
   - Jalur eksekusi (Path/Command not found)
   - Ketidaksesuaian Baris Baru (CRLF vs LF di Linux)
   - Dependensi/Versi yang hilang
2. **Coba Perbaikan Otomatis:**
   - **Masalah Hak Akses:** Di Linux/macOS, gunakan diagnostik `ls -la`. Tawarkan perbaikan izin jika berada di dalam *safe-zone*.
   - **CRLF vs LF:** Jika skrip shell gagal dengan pesan error misterius seperti `$'\r': command not found`, jalankan utility `dos2unix` atau hapus karakter carriage return (`\r`) secara otonom.
   - **Command not found:** Periksa apakah executable berada di path yang berbeda atau perlu dipanggil via `npx` / run-wrapper lainnya.
3. **Batas Toleransi (HITL Trigger):** 
   - Jika setelah **3x upaya perbaikan mandiri** masalah masih berlanjut, segera hentikan eksekusi, laporkan riwayat diagnostik secara jujur, dan mintalah intervensi pengguna (Human-in-the-Loop).

---

## 🛠️ PANDUAN PENCEGAHAN TARBOMB (EKSTRAKSI ZIP/TAR)
Setiap mengekstrak arsip di root workspace:
- **Cek Isi Dulu:** Jalankan `unzip -l` atau `tar -tf` untuk memverifikasi apakah ada folder pembungkus (*root wrapper folder*).
- **Jika Tidak Ada Folder Pembungkus:** Jangan langsung diekstrak di root. Buatkan folder khusus sesuai nama arsip terlebih dahulu, lalu ekstrak ke dalamnya untuk mencegah file berhamburan di root.
