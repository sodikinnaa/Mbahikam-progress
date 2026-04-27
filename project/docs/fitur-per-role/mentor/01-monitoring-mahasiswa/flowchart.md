# Flowchart - Mentor - Monitoring Mahasiswa

Fokus fitur ini hanya pada penggunaan mentor untuk memantau progres mahasiswa bimbingan.

```mermaid
flowchart TD
	A([Start]) --> B[Mentor login]
	B --> C[Buka menu monitoring mahasiswa]
	C --> D[Tampilkan daftar mahasiswa bimbingan]
	D --> E[Mentor pilih salah satu mahasiswa]
	E --> F[Tampilkan ringkasan presensi mahasiswa]
	F --> G[Tampilkan ringkasan status logbook]
	G --> H{Perlu detail?}
	H -->|Ya| I[Buka detail riwayat presensi dan logbook]
	I --> J[Kembali ke daftar mahasiswa]
	J --> D
	H -->|Tidak| K([End])
```

## Narasi Singkat

1. Mentor masuk ke menu monitoring untuk melihat mahasiswa yang dibimbing.
2. Mentor memilih mahasiswa lalu memantau progres presensi dan logbook.
3. Jika diperlukan, mentor membuka detail riwayat sebelum kembali ke daftar.
