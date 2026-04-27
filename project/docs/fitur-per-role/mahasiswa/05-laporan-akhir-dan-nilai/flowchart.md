# Flowchart - Mahasiswa - Laporan Akhir dan Nilai

Fokus fitur ini hanya pada unggah laporan akhir dan akses hasil nilai.

```mermaid
flowchart TD
	A([Start]) --> B[Mahasiswa buka menu laporan akhir]
	B --> C[Upload file laporan akhir PDF]
	C --> D[Sistem validasi format dan ukuran file]
	D --> E{Valid?}
	E -->|Tidak| F[Tampilkan error dan minta upload ulang]
	F --> C
	E -->|Ya| G[Simpan laporan akhir]
	G --> H[Menunggu mentor input penilaian]
	H --> I[Sistem hitung nilai akhir otomatis]
	I --> J[Mahasiswa buka menu nilai]
	J --> K[Tampilkan nilai akhir]
	K --> L([End])
```

## Narasi Singkat

1. Mahasiswa mengunggah laporan akhir dalam format yang ditentukan.
2. Sistem menyimpan laporan jika valid, lalu menunggu penilaian mentor.
3. Setelah nilai diproses, mahasiswa dapat melihat nilai akhir di sistem.
