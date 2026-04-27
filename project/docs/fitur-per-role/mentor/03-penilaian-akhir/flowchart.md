# Flowchart - Mentor - Penilaian Akhir

Fokus fitur ini hanya pada penggunaan mentor untuk input dan finalisasi penilaian akhir mahasiswa.

```mermaid
flowchart TD
	A([Start]) --> B[Mentor buka menu penilaian akhir]
	B --> C[Pilih mahasiswa bimbingan]
	C --> D[Buka form penilaian]
	D --> E[Input skor: analisis, komunikasi, kerja sama, disiplin]
	E --> F[Sistem hitung nilai akhir otomatis]
	F --> G[Mentor review ringkasan nilai]
	G --> H{Data nilai sudah benar?}
	H -->|Belum| I[Perbaiki skor pada form]
	I --> F
	H -->|Sudah| J[Submit penilaian final]
	J --> K[Sistem simpan nilai akhir mahasiswa]
	K --> L([End])
```

## Narasi Singkat

1. Mentor memilih mahasiswa dan mengisi skor tiap aspek penilaian.
2. Sistem menghitung nilai akhir secara otomatis berdasarkan skor yang diinput.
3. Mentor meninjau hasil, lalu melakukan final submit jika nilai sudah benar.
