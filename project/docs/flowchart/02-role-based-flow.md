# Flowchart Role-Based MAGIS

Dokumen ini merangkum alur utama tiap role secara terpisah namun tetap saling terhubung.

## 1. Alur Mahasiswa

```mermaid
flowchart TD
    A([Start]) --> B[Registrasi dan login]
    B --> C[Lengkapi profil dan berkas]
    C --> D[Tunggu validasi admin]
    D --> E[Presensi harian]
    E --> F[Input logbook harian]
    F --> G[Upload laporan akhir]
    G --> H[Lihat nilai akhir]
    H --> I([End])
```

## 2. Alur Admin

```mermaid
flowchart TD
    A([Start]) --> B[Kelola periode magang]
    B --> C[Validasi pendaftaran]
    C --> D[Input mahasiswa manual jika diperlukan]
    D --> E[Assign mentor]
    E --> F[Monitoring absensi]
    F --> G[Monitoring logbook]
    G --> H[Generate laporan dan export]
    H --> I([End])
```

## 3. Alur Mentor

```mermaid
flowchart TD
    A([Start]) --> B[Login mentor]
    B --> C[Monitoring mahasiswa bimbingan]
    C --> D[Validasi logbook]
    D --> E[Input penilaian akhir]
    E --> F([End])
```

## Ringkasan

1. Mahasiswa fokus pada aktivitas operasional magang.
2. Admin fokus pada kontrol proses dan administrasi.
3. Mentor fokus pada validasi aktivitas dan evaluasi akhir.
