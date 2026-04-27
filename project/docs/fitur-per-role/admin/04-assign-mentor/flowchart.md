# Flowchart - Admin - Assign Mentor

Fokus fitur ini hanya pada penetapan mentor ke mahasiswa yang sudah diterima.

```mermaid
flowchart TD
	A([Start]) --> B[Admin buka menu assign mentor]
	B --> C[Pilih mahasiswa berstatus diterima atau aktif]
	C --> D[Tampilkan daftar mentor tersedia]
	D --> E[Admin pilih mentor]
	E --> F[Sistem cek ketersediaan mentor]
	F --> G{Mentor tersedia?}
	G -->|Tidak| H[Tampilkan peringatan beban mentor]
	H --> D
	G -->|Ya| I[Simpan relasi mentor-mahasiswa]
	I --> J[Tampilkan notifikasi assign berhasil]
	J --> K([End])
```

## Narasi Singkat

1. Admin memilih mahasiswa yang perlu pembimbing.
2. Admin menetapkan mentor dari daftar mentor yang tersedia.
3. Sistem menyimpan relasi mentor-mahasiswa setelah validasi.
