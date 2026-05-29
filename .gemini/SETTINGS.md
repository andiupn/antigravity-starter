# Konfigurasi Pengaturan & Izin (Settings)

Repositori ini menggunakan sistem pengaturan dua tingkat untuk menjaga keamanan dan fleksibilitas pengembangan.

## Struktur Pengaturan

- **`.gemini/settings.json`** — Konfigurasi global proyek (dilacak oleh Git)
  - Dibagikan kepada seluruh anggota tim / kontributor.
  - Berisi daftar perkakas independen platform dan konfigurasi MCP server dasar.

- **`.gemini/settings.local.json`** — Konfigurasi lokal spesifik pengguna (diabaikan oleh Git)
  - Bersifat spesifik per mesin/perangkat pengembang.
  - Mengatur izin eksekusi perintah (seperti `git`, `npm`, dsb.) dan izin menulis berkas.
  - Berisi batasan keamanan untuk mencegah perintah destruktif seperti `rm -rf` atau `sudo`.

- **`.gemini/settings.local.example.json`** — Templat pengaturan lokal (dilacak oleh Git)
  - Menyediakan templat izin dasar untuk Linux dan Windows.

---

## Langkah Setup Awal

Untuk mengaktifkan izin bagi AI Agent di mesin Anda:

```bash
# Salin templat lokal
cp .gemini/settings.local.example.json .gemini/settings.local.json

# Buka .gemini/settings.local.json dan sesuaikan blok OS Anda.
# Ubah nama kunci dari "permissions_LINUX" atau "permissions_WINDOWS" menjadi "permissions" saja.
```

---

## Variabel Lingkungan (.env)

- **`GITHUB_TOKEN`** (Wajib jika menggunakan integrasi GitHub)
  - Digunakan untuk autentikasi server MCP GitHub.
  - Dapatkan token di: [GitHub Settings → Personal access tokens](https://github.com/settings/tokens) dengan scope `repo`.
  - Salin `.env.example` menjadi `.env` dan isi token Anda di sana.

---

## Prinsip Keamanan Agent

1. **Hak Akses Minimum (Least Privilege):** Berikan izin hanya untuk perkakas dan direktori yang benar-benar dibutuhkan.
2. **Sandboxing Tulis:** Izin menulis (`Write`) secara default dibatasi ke direktori kerja Anda (misal `./src/` atau `./.gemini/`).
3. **Pencegahan Destruktif:** Perintah berbahaya seperti `rm -rf /` atau eskalasi hak akses `sudo` diblokir secara eksplisit untuk mencegah kerusakan tidak disengaja.
