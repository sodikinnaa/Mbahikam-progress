# Flowchart - Mahasiswa - Registrasi dan Profil

Fokus fitur ini hanya pada pembuatan akun dan pelengkapan profil mahasiswa.

```mermaid
flowchart TD
    A([Start]) --> B{Sumber akun mahasiswa}

    B -->|Registrasi mandiri| C[Buka form registrasi publik]
    C --> D[Isi data akun: nama, email, NIM, universitas, password]
    D --> E[Sistem validasi format dan kelengkapan]
    E --> F{Data valid?}
    F -->|Tidak| G[Tampilkan error dan minta perbaikan]
    G --> D
    F -->|Ya| H[Sistem buat akun]
    H --> I[Kirim verifikasi email atau notifikasi berhasil]

    B -->|Akun dari admin| J[Mahasiswa menerima kredensial awal]

    I --> K[Mahasiswa login]
    J --> K
    K --> L[Lengkapi profil: prodi, no telepon, alamat]
    L --> M[Simpan profil]
    M --> N{Profil lengkap?}
    N -->|Belum| L
    N -->|Sudah| O([End: Akun dan profil siap])
```

## Narasi Singkat

1. Mahasiswa bisa memperoleh akun lewat registrasi mandiri atau akun yang dibuat admin.
2. Pada jalur mandiri, sistem memvalidasi data sebelum akun dibuat.
3. Setelah akun tersedia, mahasiswa login dan melengkapi data profil.
4. Alur selesai saat profil sudah lengkap dan siap dipakai ke fitur pendaftaran.
