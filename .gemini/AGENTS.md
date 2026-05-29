# Agen AI: Asisten Spesialis Antigravity

Agen AI adalah **instansi asisten spesialis** yang dapat dipanggil untuk menangani tugas tertentu dengan lebih efisien, hemat biaya, dan terisolasi dari riwayat obrolan sesi utama.

## Daftar Agen

Dalam templat starter ini, hanya terdapat **2 agen utama** yang telah dinonaktifkan konfigurasi *thinking*-nya agar berjalan cepat dan hemat token menggunakan model **Gemini 3.5 Flash**:

1. **`code-reviewer`**
   - **Tujuan:** Memeriksa kualitas kode, mendeteksi bug, dan memastikan kepatuhan terhadap standar pengodean (`coding_standards.md`).
   - **Cara Memanggil:** `@code-reviewer` atau melalui panggilan UI chat.
   - **Kapan Digunakan:** Sebelum melakukan komit kode atau ketika ingin memverifikasi potongan kode tertentu.

2. **`research-assistant`**
   - **Tujuan:** Melakukan riset teknis, mencari dokumentasi API, membandingkan pustaka, dan membantu pengambilan keputusan teknologi.
   - **Cara Memanggil:** `@research-assistant` atau melalui panggilan UI chat.
   - **Kapan Digunakan:** Sebelum mulai menulis kode baru atau ketika mempelajari pola arsitektur baru.

---

## Panduan Penggunaan Agen

### Cara Memanggil di Chat UI
Cukup sebut nama agen di awal pesan Anda:
```markdown
@research-assistant: Apa perbedaan utama antara Tailwind v3 dan Tailwind v4 dalam hal performa build?
```
```markdown
@code-reviewer: Tolong periksa berkas src/index.ts ini apakah sudah memenuhi standar TypeScript strict.
```

### Isolasi Konteks
Setiap pemanggilan agen bersifat **mandiri** dan **terisolasi**:
- Agen **tidak dapat melihat** riwayat sesi utama Anda secara otomatis.
- Jika tugas agen membutuhkan konteks berkas atau memori proyek, sertakan informasi penting tersebut ke dalam prompt Anda secara eksplisit, atau instruksikan agen untuk membaca berkas tertentu di dalam `./src`.
