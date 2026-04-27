# Flowchart Global MAGIS

Dokumen ini menggambarkan alur global sistem MAGIS dari pendaftaran hingga pelaporan akhir.

```mermaid
flowchart TD
    A([Start]) --> B[Mahasiswa registrasi atau akun dibuat admin]
    B --> C[Mahasiswa lengkapi profil dan berkas]
    C --> D[Admin validasi pendaftaran]
    D --> E{Diterima?}
    E -->|Tidak| F[Status ditolak dengan alasan]
    F --> Z([End])
    E -->|Ya| G[Admin assign mentor]
    G --> H[Mahasiswa aktif mulai magang]
    H --> I[Mahasiswa presensi harian check-in dan check-out]
    I --> J[Mahasiswa isi logbook harian]
    J --> K[Mentor validasi logbook]
    K --> L{Perlu revisi?}
    L -->|Ya| J
    L -->|Tidak| M[Mahasiswa upload laporan akhir]
    M --> N[Mentor input penilaian akhir]
    N --> O[Admin monitoring dan generate laporan]
    O --> P[Export laporan PDF atau Excel]
    P --> Z
```

## Ringkasan

1. Alur dimulai dari onboarding mahasiswa.
2. Proses operasional utama meliputi presensi, logbook, dan validasi mentor.
3. Alur ditutup dengan penilaian akhir serta pelaporan administratif oleh admin.
