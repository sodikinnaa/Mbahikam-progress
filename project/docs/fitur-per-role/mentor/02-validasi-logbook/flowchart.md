# Flowchart - Mentor - Validasi Logbook

Fokus fitur ini hanya pada penggunaan mentor untuk memvalidasi logbook harian mahasiswa.

```mermaid
flowchart TD
   A([Start]) --> B[Mentor buka antrean logbook pending]
   B --> C[Pilih logbook mahasiswa]
   C --> D[Review deskripsi kegiatan dan lampiran bukti]
   D --> E{Sesuai?}
   E -->|Ya| F[Pilih aksi setujui]
   F --> G[Sistem update status logbook: Disetujui]
   G --> H([End])
   E -->|Tidak| I[Pilih aksi tolak]
   I --> J[Isi komentar revisi wajib]
   J --> K[Sistem update status logbook: Ditolak]
   K --> L[Logbook kembali ke mahasiswa untuk perbaikan]
   L --> H
```

## Narasi Singkat

1. Mentor membuka antrean logbook yang menunggu validasi.
2. Mentor meninjau isi aktivitas dan lampiran bukti mahasiswa.
3. Mentor menyetujui jika sesuai, atau menolak dengan komentar revisi jika belum sesuai.
