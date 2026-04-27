# Flowchart - Admin - Monitoring Absensi

Fokus fitur ini hanya pada pemantauan data kehadiran mahasiswa oleh admin.

```mermaid
flowchart TD
	A([Start]) --> B[Admin buka dashboard monitoring absensi]
	B --> C[Pilih filter periode dan tanggal]
	C --> D[Sistem tampilkan rekap check-in dan check-out]
	D --> E[Admin review data kehadiran]
	E --> F{Ada anomali absensi?}
	F -->|Ya| G[Tandai mahasiswa dengan absensi bermasalah]
	G --> H[Buka detail riwayat absensi mahasiswa]
	H --> I[Kembali ke dashboard absensi]
	I --> C
	F -->|Tidak| J([End])
```

## Narasi Singkat

1. Admin memfilter data absensi berdasarkan periode dan tanggal.
2. Sistem menampilkan rekap kehadiran untuk ditinjau.
3. Jika ditemukan anomali, admin membuka detail riwayat untuk pemeriksaan lanjut.
