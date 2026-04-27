# Flowchart - Mahasiswa - Logbook Harian

Fokus fitur ini hanya pada pengisian logbook dan siklus revisi validasi mentor.

```mermaid
flowchart TD
	A([Start]) --> B[Mahasiswa buka menu logbook harian]
	B --> C[Isi deskripsi kegiatan]
	C --> D[Upload bukti foto atau dokumen]
	D --> E[Submit logbook]
	E --> F[Sistem set status: Menunggu Validasi Mentor]
	F --> G{Hasil validasi mentor}
	G -->|Ditolak| H[Mahasiswa menerima catatan revisi]
	H --> I[Mahasiswa perbaiki isi logbook]
	I --> E
	G -->|Disetujui| J[Sistem set status: Disetujui]
	J --> K([End: Logbook valid])
```

## Narasi Singkat

1. Mahasiswa mengisi aktivitas harian dan mengunggah bukti pendukung.
2. Logbook dikirim dengan status menunggu validasi mentor.
3. Jika ditolak, mahasiswa revisi lalu kirim ulang sampai disetujui.
