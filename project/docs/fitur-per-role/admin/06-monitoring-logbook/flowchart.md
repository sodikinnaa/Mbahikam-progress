# Flowchart - Admin - Monitoring Logbook

Fokus fitur ini hanya pada pemantauan progres logbook mahasiswa oleh admin.

```mermaid
flowchart TD
	A([Start]) --> B[Admin buka dashboard monitoring logbook]
	B --> C[Pilih filter periode, mahasiswa, atau status]
	C --> D[Sistem tampilkan daftar logbook dan status validasi]
	D --> E[Admin identifikasi logbook pending atau belum diisi]
	E --> F{Perlu detail aktivitas?}
	F -->|Ya| G[Buka detail logbook mahasiswa]
	G --> H[Kembali ke dashboard logbook]
	H --> C
	F -->|Tidak| I([End])
```

## Narasi Singkat

1. Admin memantau logbook menggunakan filter status dan periode.
2. Sistem menampilkan logbook yang sudah divalidasi maupun yang masih pending.
3. Admin dapat membuka detail untuk melihat kendala pengisian logbook.
