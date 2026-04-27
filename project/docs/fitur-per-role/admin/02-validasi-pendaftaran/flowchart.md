# Flowchart - Admin - Validasi Pendaftaran

Fokus fitur ini hanya pada proses admin saat memvalidasi pendaftaran mahasiswa.

```mermaid
flowchart TD
   A([Start]) --> B[Admin buka daftar pendaftaran]
   B --> C[Pilih pengajuan pendaftaran]
   C --> D[Review data profil dan berkas syarat]
   D --> E{Berkas lengkap dan sesuai?}
   E -->|Ya| F[Pilih aksi terima]
   F --> G[Sistem ubah status: Diterima]
   G --> H([End])
   E -->|Tidak| I[Pilih aksi tolak]
   I --> J[Isi alasan penolakan]
   J --> K[Sistem ubah status: Ditolak]
   K --> H
```

## Narasi Singkat

1. Admin memeriksa pengajuan berdasarkan data dan kelengkapan berkas.
2. Jika sesuai, admin menerima pendaftaran.
3. Jika tidak sesuai, admin menolak dengan alasan yang tercatat.
