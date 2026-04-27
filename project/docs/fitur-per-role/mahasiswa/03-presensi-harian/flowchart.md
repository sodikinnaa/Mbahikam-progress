# Flowchart - Mahasiswa - Presensi Harian

Fokus fitur ini hanya pada alur presensi masuk dan presensi pulang.

```mermaid
flowchart TD
	A([Start]) --> B[Mahasiswa pilih presensi masuk]
	B --> C[Ambil selfie dan timestamp]
	C --> D[Ambil lokasi GPS opsional]
	D --> E[Sistem validasi data presensi masuk]
	E --> F{Valid?}
	F -->|Tidak| G[Tampilkan gagal presensi, minta ulang]
	G --> C
	F -->|Ya| H[Simpan check-in]
	H --> I[Mahasiswa menjalankan aktivitas harian]
	I --> J[Mahasiswa pilih presensi pulang]
	J --> K[Ambil selfie dan timestamp pulang]
	K --> L[Sistem validasi data presensi pulang]
	L --> M{Valid?}
	M -->|Tidak| N[Tampilkan gagal presensi pulang, minta ulang]
	N --> K
	M -->|Ya| O[Simpan check-out]
	O --> P([End: Presensi harian lengkap])
```

## Narasi Singkat

1. Mahasiswa melakukan check-in dengan bukti selfie dan waktu.
2. Sistem memvalidasi data sebelum menyimpan presensi masuk.
3. Di akhir hari, mahasiswa melakukan check-out dengan proses validasi yang sama.
