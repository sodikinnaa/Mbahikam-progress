# Flowchart - Admin - Laporan dan Export

Fokus fitur ini hanya pada pembuatan laporan dan proses export data oleh admin.

```mermaid
flowchart TD
	A([Start]) --> B[Admin buka menu laporan dan export]
	B --> C[Pilih jenis laporan]
	C --> D[Pilih periode laporan]
	D --> E[Sistem generate rekap data]
	E --> F{Data berhasil digenerate?}
	F -->|Tidak| G[Tampilkan pesan gagal generate]
	G --> C
	F -->|Ya| H[Pilih format export: PDF atau Excel]
	H --> I[Sistem buat file laporan]
	I --> J[Admin unduh file laporan]
	J --> K([End])
```

## Narasi Singkat

1. Admin memilih jenis laporan dan periode data yang dibutuhkan.
2. Sistem membentuk rekap data sesuai filter.
3. Admin mengekspor hasil ke PDF atau Excel untuk kebutuhan pelaporan.
